
 node('windows-slave') {
    stage ('Checkout') {
        git branch: 'master',
        credentialsId: '8ecbfffb-7a57-429c-90d2-8807d902dd99',
        url: 'https://github.com/MerrilCode/sample-net-app.git'
    }

    stage ('Build'){
        bat 'nuget restore helloworld.sln'
        bat "\"${tool 'MSBuild'}\" helloworld.sln /p:Configuration=Release /p:Platform=\"Any CPU\" /p:ProductVersion=1.0.0.${env.BUILD_NUMBER}"
    }
    
        

}