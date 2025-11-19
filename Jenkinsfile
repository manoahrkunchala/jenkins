pipeline{
    agent any
        stages{
            stage('build'){
                steps{
                    echo 'build is running'
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