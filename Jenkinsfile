pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                git url: 'https://github.com/20127589/newtest.git', branch: '*'
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
