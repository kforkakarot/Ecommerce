node('ec2'){
    stage('Checkout') {
        steps{
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
    }
    
    stage('Build') {
        steps{
            dir("files")
            {
                sh "ls"
            }
        }
    }
    
    stage('Deploy') {
        steps{
            sh 'echo deploy'
        }
    }

}
