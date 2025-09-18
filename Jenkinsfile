pipeline {
    agent any

    stages {

        stage("Build") {
            options {
                timeout(time: 1, unit: 'HOURS')
                timestamps()
            }
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
        always {
            echo "Cette étape est toujours exécuté"
        }
        success {
            echo "Cette étape est exécuté en cas des succès"
        }
    }
}