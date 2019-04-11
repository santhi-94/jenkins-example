pipeline {
    agent none

    stages {
        stage ('Compile Stage') {

            steps {
                   maven(maven : 'maven_3.3.3') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                maven(maven : 'maven_3.3.3') {
                    sh 'mvn test'
                }
            }
        }


        stage ('Deployment Stage') {
            steps {
                  maven(maven : 'maven_3.3.3') {
                    sh 'mvn deploy'
                }
            }
        }
    }
}
