pipeline {
    agent any 

    triggers {
        pollSCM('* * * * *')
    }

    // parameters {
    //     string(name: "PERSONNE", defaultValue:"M. ABAKAR", description: "A qui devrais-je dire bonjour ?")
    //     text(name: "BIOGRAPHIE", defaultValue: "", description: "Entrez des informations sur la personne")
    //     booleanParam(name: "TOGGLE", defaultValue: true, description: "Activez cette valeur")
    //     choice(name: "CHOIX", choices: ["Un", "Deux", "Trois"], description: "Faites un chooix")
    //     password(name: "MOT_DE_PASSE", defaultValue: "SECRET", description: "Entrez un mot de passe")
    // }

    stages {

        stage("Exemple") {

            steps {
                // echo "Bonjour ${PERSONNE}"
                // echo "Biographie ${BIOGRAPHIE}"
                // echo "Toggle ${TOGGLE}"
                // echo "Choix ${CHOIX}"
                // echo 'Mot de passe ${MOT_DE_PASSE}'
                echo "Ceci est un exemple"
            }

        }

    }

    post {
        always {
            echo "Cette étape est toujours exécuté"
        }
        success {
            echo "Cette étape est exécuté en cas du succès"
        }
        failure {
            echo "Cette étape est exécuté en cas d'échec"
        }
    }
}



// A récupérer si besoin
// pipeline {
//     agent any

//     parametres {
//         text()

//     }

//     stages {

//         stage("Build") {
//             options {
//                 timeout(time: 1, unit: 'HOURS')
//                 timestamps()
//             }
//             steps {
//                 echo "Construire le projet"
//             }
//         }

//         stage("Test") {
//             steps {
//                 echo "Tester le projet"
//             }
//         }

//     }

//     post {
//         always { 
//             echo "Cette étape est toujours exécuté"
//         }
//         success {
//             echo "Cette étape est exécuté en cas des succès"
//         }
//     }
// }