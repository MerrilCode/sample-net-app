
node('windows-slave') {
    stage "checkout"
    //git([url:"https://github.com/MerrilCode/sample-net-app.git"])
    checkout([$class: 'GitSCM', 
        branches: [[name: '*/master']], 
        doGenerateSubmoduleConfigurations: false, 
        extensions: [[$class: 'RelativeTargetDirectory', 
            relativeTargetDir: 'checkout-directory']], 
        submoduleCfg: [], 
        userRemoteConfigs: [[url: 'https://github.com/MerrilCode/sample-net-app.git']]])

    stage "build"
    echo "Building from pipeline"
}