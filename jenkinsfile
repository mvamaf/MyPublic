pipeline {
    agent any
    
    environment {
        PROJECT_NAME = 'MY-PROJECT-GITHUB'
        OWNER_NAME   = 'MVA'
    }

    stages {
        stage('STAGE-BUILD') {
            steps {
                echo 'Start of Stage Build'
                echo 'Building ......'
                echo 'End of Stage Build'
            }
        }
        stage('STAGE-TEST'){
            steps {
                echo 'Start of stage Test'
                echo 'Testing ......'
                sh 'ls -la /tmp'
                echo "Hello ${OWNER_NAME}"
                echo "Project name is ${PROJECT_NAME}"
                echo 'End of stage Test'
            }
        }
        stage('STAGE-DEPLOY') {
            steps {
                echo 'Start of Stage Deploy'
                echo 'Deploying.........'
                sh '''
                     echo 'Line 1'
                     echo 'Line 2'
                     echo 'Line 3'
                '''
                echo 'End of Stage Deploy'
            }
        }
    }
}

