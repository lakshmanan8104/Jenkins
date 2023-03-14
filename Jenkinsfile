pipeline{
    agent any
    environment{
        staging_server="172.31.32.229"
    }
    stages{
        stage('Deploy to Remote'){
            steps{
              sh ' scp -r /var/lib/jenkins/workspace/jenkins/* jenkins@172.31.32.229:/home/ubuntu/'
              
              }
        }
    }
}
