pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Code récupéré avec succès'
            }
        }

        stage('Build') {
            steps {
                echo 'Build simulé (pas de Maven)'
            }
        }

        stage('Test') {
            steps {
                echo 'Tests simulés'
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
