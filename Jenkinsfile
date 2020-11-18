pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                 sh 'docker build -t kartikeya390/perl:Latest1 .'
            }
        }
        stage('Test') {
            steps {
                withCredentials([string(credentialsId: 'kartikeya390', variable: 'docker-paswd')]) {
                sh "docker login --username kartikeya390 --password {$docker-paswd}"
            }
        }
      }
        stage('Deploy') {
            steps {
                sh 'docker push kartikeya390/jenkins-007:latest1'
            }
        }
    }
}
