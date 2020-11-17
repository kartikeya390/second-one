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
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
