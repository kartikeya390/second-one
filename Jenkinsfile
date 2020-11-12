pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                 docker ps-a
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
