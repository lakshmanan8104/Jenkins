pipeline{
    agent any
    environment{
        staging_server="172.31.1.171"
    }
    stages{
        stage('Deploy to Remote'){
            steps{
              sh 'scp -r /var/lib/jenkins/workspace/* ubuntu@172.31.1.171:/home/ubuntu/'
              }
        }
    }
}
