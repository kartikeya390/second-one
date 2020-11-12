pipeline {

     agent any  

        stage('Building our image') { 

            steps { 

                script { 

                    docker run -dit -p 80:80 httpd
                    docker ps-a
                }

            } 

        }

    }




