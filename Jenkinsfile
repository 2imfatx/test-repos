pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                git 'https://github.com/20127589/newtest.git'
                sh 'mvn clean install'
            }
        }
        stage('Deploy') {
            steps {
                sh './deploy.sh'
            }
        }
    }
}
