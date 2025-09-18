pipeline {
    agent none
    stages {

        stage("Exemple de build") {
            agent {
                docker 'maven:3.9.3-eclipse-temurin-17'
            }
            steps {
                echo 'Hello, Maeven'
                sh "mvn --version"
            }
        }
        
        stage('Example de Test') {
            agent {
                docker 'openjdk:17-jre'
            }
            steps {
                echo 'Hello, JDK'
                sh 'java --version'
            }
        }
    }
}