pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'docker build -t vampir/spring-app:latest .'
            }
        }
        stage('Push') {
            steps {
                sh 'docker login && docker push vampir/spring-app:latest'
            }
        }
    }
}