node {
        stage('Clone GitHub') {
            
                git branch: 'develop', credentialsId: 'credential', url: 'https://github.com/pabsdevops/maven-web-app.git'
            
        }
        
        stage('Maven Build') {
           
                sh 'mvn clean package'
            
        }
}
