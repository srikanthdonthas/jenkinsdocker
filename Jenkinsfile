pipeline {
    agent any
    stages {
        stage('Build') {
            agent {
                docker {
                    image 'gradle:6.7-jdk11'
                    // Run the container on the node specified at the
                    // top-level of the Pipeline, in the same workspace,
                    // rather than on a new node entirely:
                    reuseNode true
                }
            }
            steps {
                sh 'gradle --version'
            }
        }
    }
}




// pipeline {
//     agent any
//     stages {
//         stage('docker') {
//             agent {
//                 docker { image 'node:16.13.1-alpine' }
//             }
//             steps{
//                 sh '''
//                     docker -v
                
//                 '''
//             }
//         }
        // stage('Build') {
        //     steps{
        //         sh '''
        //             docker build -t helo_there
        //         '''
        //     }
        // }
        // stage('run') {
        //     steps{
        //         sh '''
        //             docker run --rm helo_there
        //         '''
        //     }
        // }
//     }
// }