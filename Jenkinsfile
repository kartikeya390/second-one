pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                 chmod -r 755 NVM\&docker_2020.sh
                 sh 'docker images'
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
