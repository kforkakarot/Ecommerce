pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                sh 'echo checking out'
            }
        }
        
        stage('Build') {
            steps {
                sh 'echo Building'
                }
        }
        
        stage('Deploy') {
            steps {
                sh 'echo deploying'
                }
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
