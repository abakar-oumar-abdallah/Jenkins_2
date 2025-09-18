pipeline {
    agent any

    stages {

        stage("Build") {
            steps {
                echo "Construire le projet"
                sh 'make build'
            }
        }

        stage("Test") {
            steps {
                echo "Tester le projet"
            }
        }

    }

    post {
        always {
            echo "Cette étape est toujours exécuté"
        }
        success {
            echo "Cette étape est exécuté en cas des succès"
        }
    }
}