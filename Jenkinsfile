pipeline {
    agent any
    tools {
        maven '3.8.7'
    }
    stages {
        stage('Build') {
            steps {
                git branch: 'main', credentialsId: 'git', url: 'https://github.com/2imfatx/test-repos.git'
                
                sh 'mvn --version'
            }
        }
    }
}
