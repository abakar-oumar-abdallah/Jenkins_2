pipeline {
    agent any

    stages {

        stage("Test") {
            steps {
                echo "Tester le projet pour voir la section Post ce qui va nous donner"

            }
        }
    }

    post {
        always {
            echo "Cette étape est toujours exécuté"
        }
        success {
            echo "Cette étae est exécuté en cas des succès"
        }
    }
}