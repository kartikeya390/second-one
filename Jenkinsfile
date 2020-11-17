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
                sh "docker login -u kartikeya390 -p {$docker-paswd}"
            }
        }
      }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
