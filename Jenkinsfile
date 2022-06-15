pipeline {
    agent any
    stages {
        stage('docker') {
        agent {
                docker { build . -t helo_there }
            }
            steps{
                sh '''
                    docker -v
                
                '''
            }
        }
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
    }
}