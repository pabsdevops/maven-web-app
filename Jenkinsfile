node{
    
    stage('Clone repo'){
        git credentialsId: 'credential', url: 'https://github.com/pabsdevops/maven-web-app.git'
    }
    
    stage('Maven Build'){
        def mavenHome = tool name: "Maven-3.6.3", type: "maven"
        def mavenCMD = "${mavenHome}/bin/mvn"
        sh "${mavenCMD} clean package"
    }
    
}
