pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                script {
                    docker.image('node:12').inside('-u root') {
                        sh 'npm install'
                    }
                }
            }
        }
//         stage('Test') {
//             steps {
//                 sh './jenkins/scripts/test.sh'
//             }
//         }
    }
}