pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven 'mvn_3_5_4') {
                    sh 'mvn clean compile'
                    echo 'compile complete'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withMaven(maven 'mvn_3_5_4') {
                    sh 'mvn test'
                    echo 'test complete'                    
                }
            }
        }

        stage ('Deployment Stage') {
            steps {
                withMaven(maven 'mvn_3_5_4') {
                    sh 'mvn deploy'
                    echo 'deploy complete'
                }
            }
        }
    }
}
