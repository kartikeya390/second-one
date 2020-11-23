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
                withCredentials([usernameColonPassword(credentialsId: 'Docker-user-pass', variable: 'Docker-user-passwd')]) {
                 sh "docker login --username kartikeya390 --password-stdin {$docker-paswd}"
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
