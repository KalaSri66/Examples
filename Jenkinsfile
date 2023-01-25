pipeline {
    agent any

    environment {
      CC = 'clang'
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
                sh 'printenv'
            }
        }
    }
}
