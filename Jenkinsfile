
 node('windows-slave') {
    stage('Checkout external proj') {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '8ecbfffb-7a57-429c-90d2-8807d902dd99', url: 'https://github.com/MerrilCode/sample-net-app.git']]])
    }
        

}