pipeline {
    agent none

    stages {
        stage ('Compile Stage') {

            steps {
                   Maven(maven : 'maven_3.3.3') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                Maven(maven : 'maven_3.3.3') {
                    sh 'mvn test'
                }
            }
        }


        stage ('Deployment Stage') {
            steps {
                  Maven(maven : 'maven_3.3.3') {
                    sh 'mvn deploy'
                }
            }
        }
    }
}
