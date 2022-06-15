pipeline {
    agent any
    stages {
        stage('Build') {
            steps{
                sh """"
                    docker build -t helo_there
                """
            }
        }
        stage('run') {
            steps{
                sh """"
                    docker run --rm helo_there
                """
            }
        }
    }
}