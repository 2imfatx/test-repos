pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                git branch: 'main', credentialsId: 'git', url: 'https://github.com/2imfatx/test-repos.git'

                sh 'apt-get update'
                sh 'apt-get install maven -y'
                sh 'mvn --version'
            }
        }
    }
}
