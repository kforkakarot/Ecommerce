node('ec2'){
    stage('Checkout') {
        dir("files"){
                script {
                checkout([$class: 'GitSCM', 
                    branches: [[name: '*/main']],
                    doGenerateSubmoduleConfigurations: false,
                    extensions: [[$class: 'CleanCheckout'], [$class: 'CloneOption', shallow: true, noTags: true, reference: '', timeout: 10]],
                    userRemoteConfigs: [[url: 'https://github.com/kforkakarot/Ecommerce.git']]
                ])
            }
        }
    }
    
    stage('Build') {
        dir("files")
        {
            sh "ls"
        }
    }
    
    stage('Deploy') {
        sh 'echo deploy'
    }

}
