pipeline{
    agent {
        label 'AGENT-1'
    }
    environment{
        COURSE = 'jenkins'
    }
    options { 
        timeout(time: 10, unit: 'SECONDS') 
    }
    stages{
        stage('build'){
            steps{
                script{
                    sh """
                        echo 'build is running'
                        env
                    """
                }
            }
        }
        stage('test'){
            steps{
                echo 'test has started'
            }
        }
        stage('deploy'){
            steps{
                echo 'deploy will be begin'
            }
        }
    }
    post{
        always{
            echo 'hello team'
            deleteDir()
        }
        success{
            echo 'hello team'
        }
        failure{
            echo 'hello team'
        }
    }
}

// pipeline {
//     agent any
//     stages {
//         stage('Build') {
//             steps {
//                 //
//             }
//         }
//         stage('Test') {
//             steps {
//                 //
//             }
//         }
//         stage('Deploy') {
//             steps {
//                 //
//             }
//         }
//     }
// }