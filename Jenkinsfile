pipeline {
    agent none
     tools {
        maven 'Maven_3.3.3' 
    }
    stages {
        stage ('Compile Stage') {
            steps {
                    bat 'mvn clean compile'
            }
        }

        stage ('Testing Stage') {
            steps {
                    bat 'mvn test'
                }
            }
       stage ('Deployment Stage') {
            steps {
                    bat 'mvn deploy'
                }
            }
        }
    }
