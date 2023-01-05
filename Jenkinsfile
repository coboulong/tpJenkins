pipeline {
   
    agent any
   
    stages {

        stage('get code from github with webhook..') {
            steps {
                echo 'Pulling...';
                git branch: 'master',
                url : 'https://github.com/coboulong/tpJenkins.git';
            }

            post {
                success {
                    echo "====++++success++++===="
                }
               
                failure {
                    echo "====++++failed++++===="
                }
            }
           
        }
           
    }
}