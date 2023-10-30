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
                sh 'echo success'
        }
        failure {
                sh 'echo fail'
        }
    }
}
