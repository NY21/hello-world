pipeline {
    agent any
    
    tools { 
        maven 'mvn_3_5_4'
        jdk 'JDK_10_0_2'
    }
    
    stages {
        stage ('Initialize') {
            steps {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                ''' 
            }
        }
        
        stage ('Compile Stage') {

            steps {
                    echo 'compile complete'
            }
        }

        stage ('Testing Stage') {

            steps {
                    echo 'test complete'                    
            }
        }

        stage ('Deployment Stage') {
            steps {
                    echo 'deploy complete'
            }
        }
    }
}
