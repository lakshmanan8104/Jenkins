pipeline{
    agent any
    environment{
        staging_server="172.31.6.139"
    }
    stages{
        stage('Deploy to Remote'){
            steps{
              sh ' scp -r /var/lib/jenkins/workspace/jenkins/* jenkins@172.31.6.139:/home/ubuntu/'
              
              }
        }
    }
}
