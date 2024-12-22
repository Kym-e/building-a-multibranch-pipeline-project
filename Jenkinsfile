pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            agent {
                docker {
                    image 'node:12'
                    args '-u root'
                }
            }
            steps {
                sh 'npm install'
            }
        }
//         stage('Test') {
//             steps {
//                 sh './jenkins/scripts/test.sh'
//             }
//         }
    }
}