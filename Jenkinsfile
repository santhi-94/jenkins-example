pipeline {
    agent none
     tools {
         maven "3.3.3"
    }
    stages {
        stage ('Compile Stage') {
            steps {
                    sh 'mvn clean compile'
            }
        }

        stage ('Testing Stage') {
            steps {
                    sh 'mvn test'
                }
            }
       stage ('Deployment Stage') {
            steps {
                    sh 'mvn deploy'
                }
            }
        }
    }
