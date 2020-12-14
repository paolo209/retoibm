pipeline {
    environment {
        PATH = "$PATH:/usr/local/bin"
    }
    agent any
    stages {
        stage('build') {
            steps {
                sh '''
                docker-compose up -d
                '''
            }
        }
    }
}