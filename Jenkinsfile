pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                script {
                    def mvnHome = tool name: 'mavenTest', type: 'maven'
                    sh "${mvnHome}/bin/mvn clean compile"
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    def mvnHome = tool name: 'mavenTest', type: 'maven'
                    sh "${mvnHome}/bin/mvn test"
                }
            }
        }
    }
    post {
        success {
            echo 'Build SUCCESS ✅'
        }
        failure {
            echo 'Build FAILED ❌'
        }
    }
}
