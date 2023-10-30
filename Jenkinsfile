pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps{
                sh 'echo checkout'
            }
        }
        
        stage('Build') {
            steps{
                sh 'echo build'
            }
        }
        
        stage('Deploy') {
            steps{
                sh 'echo deploy'
            }
        }
    }
    
    post {
        success {
            steps{
                sh 'echo success'
            }
        }
        failure {
            steps{
                sh 'echo fail'
            }
        }
    }
}
