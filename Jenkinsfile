node {
    agent any

    stages {
        stage('Clone GitHub') {
            steps {
                git branch: 'develop', credentialsId: 'credential', url: 'https://github.com/pabsdevops/maven-web-app.git'
            }
        }
        
        stage('Maven Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
