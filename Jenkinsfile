pipeline {
    agent any

    stages {

        stage("Test") {
            steps {
                echo "Tester le projet pour voir la section Post ce qui va nous donner"

            }
        }

        post {
            always {
                echo "Cette étape sera toujours exécuté"
            }
            success {
                echo "Cette étape sera exécuté en cas de réussite"
            }
        }

    }
}