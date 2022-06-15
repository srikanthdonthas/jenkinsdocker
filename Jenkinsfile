pipeline {
    agent {
        docker { image 'node:16.13.1-alpine' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
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