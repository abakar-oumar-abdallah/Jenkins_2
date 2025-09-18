pipeline {
    agent any

    stages {

        stage("Build") {
            steps {
                echo "Construire le projet"
            }
        }

        stage("Test") {
            steps {
                echo "Tester le projet"
            }
        }

    }

    post {
        alwawys {
            echo "Cette étape est toujours exécuté"
        }
        success {
            echo "Cette étape est exécuté en cas des succès"
        }
    }
}