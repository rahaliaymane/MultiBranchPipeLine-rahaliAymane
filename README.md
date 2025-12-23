MultiBranchPipeLine-rahaliAymane

## Présentation du projet

Ce dépôt GitHub présente la mise en œuvre d’un **Pipeline Jenkins Multibranch** permettant d’automatiser le processus d’intégration continue (CI).
Le pipeline est déclenché automatiquement pour chaque branche du dépôt et exécute les étapes de **build** et de **validation** du projet.

Le pipeline est défini dans un fichier **Jenkinsfile** versionné directement dans le dépôt.



## 🧾 Informations générales

* **Nom du dépôt** : `MultiBranchPipeLine-rahaliAymane`
* **Outil CI/CD** : Jenkins (Multibranch Pipeline)
* **Gestion de version** :  GitHub
* **Pipeline** : Jenkinsfile (Pipeline déclaratif)

---

## ⚙️ Prérequis

Pour exécuter ce projet, il est nécessaire d’avoir :

* Java installé (selon la version du projet)
* Maven (si projet Maven)
* Jenkins configuré
* Accès GitHub depuis Jenkins

---

## ✅ Compilation du projet

Le projet a été testé et **compile sans erreur**.
La compilation est automatiquement exécutée par Jenkins à chaque push sur une branche.

Exemple de commande utilisée :

```bash
mvn clean install
```

---

## 📄 Jenkinsfile

Le fichier **`Jenkinsfile`** est présent à la racine du projet.


## 📊 Exécution du Pipeline Jenkins

Le pipeline s’exécute automatiquement pour chaque branche détectée par Jenkins.

### 🔹 Capture 1 : Détection des branches

![Détection des branches](images/branches.png)

### 🔹 Capture 2 : Exécution du pipeline

![Exécution du pipeline](images/pipeline-run.png)

### 🔹 Capture 3 : Pipeline réussi

![Pipeline réussi](images/success.png)




