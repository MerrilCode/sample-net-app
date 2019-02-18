
node('windows-slave') {

    stage 'Build'
        bat 'nuget restore helloworld.sln'
        bat "\"${tool 'MSBuild'}\" helloworld.sln /p:Configuration=Release /p:Platform=\"Any CPU\" /p:ProductVersion=1.0.0.${env.BUILD_NUMBER}"

}