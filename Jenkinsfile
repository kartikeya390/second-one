pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                 docker run -dit -p 80:80 httpd
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
