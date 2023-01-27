pipeline {
    agent any


    environment {
      CC = 'clang'
      USER_CRED = credentials('USER1_CRED')
    }
    stages {
        stage('Build') {
            environment {
               STAGEE = 'Building'
            }
            steps {
                echo 'Building..'
                sh 'printenv'
                
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                echo "${USER_CRED}"
            }
        }
    }
}
