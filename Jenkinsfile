pipeline {
    agent none
     tools {
        maven "Maven 3.3.3" 
         jdk "jdk8"
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
