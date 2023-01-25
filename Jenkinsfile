pipeline {
    agent any

    parameters {
      choice(choices: 'no\nyes', description: 'Force rebuild? To force building [ci skip] commits', name: 'FORCE_ACTION')
      choice(choices: 'yes\nno', description: 'Reset Network at start?', name: 'RESET_ACTION')
      choice(choices: 'no\nyes', description: 'Reset Only? Use this to reset only after manual testing or failure.', name: 'RESETONLY_ACTION')
      choice(choices: '2_2_2\n1_4_4', description: 'What is the Fabric version?', name: 'FABRIC_VERSION')
      choice(choices: 'raft\nkafka', description: 'What is the Fabric Consensus?', name: 'FABRIC_CONSENSUS')
      choice(choices: '4_7\n4_4', description: 'What is the Corda version?', name: 'CORDA_VERSION')
      choice(choices: '21_4_2\n2_5_0', description: 'What is the Quorum version?', name: 'QUORUM_VERSION')
      choice(choices: 'ibft\nraft', description: 'What is the Quorum Consensus?', name: 'QUORUM_CONSENSUS')
      choice(choices: 'tessera\norion', description: 'What is the Quorum/Besu TM?', name: 'QUORUM_TM')
      choice(choices: '1_12_1\n1_11_0', description: 'What is the Indy version?', name: 'INDY_VERSION') 
      choice(choices: '21_1_1\n1_5_5', description: 'What is the Besu version?', name: 'BESU_VERSION')   
    }

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
