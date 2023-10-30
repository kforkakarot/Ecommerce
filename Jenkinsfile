pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            sh 'echo checkout'
        }
        
        stage('Build') {
            sh 'echo build'
        }
        
        stage('Deploy') {
            sh 'echo deploy'
        }
    }
    
    post {
        success {
            sh 'echo Success'
            }
        failure {
            sh 'echo Failure'
            }
    }
}
