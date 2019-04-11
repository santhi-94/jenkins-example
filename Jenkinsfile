pipeline {
    agent none
     tools {
        maven "Maven 3.3.3" 
         jdk "jdk8"
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
