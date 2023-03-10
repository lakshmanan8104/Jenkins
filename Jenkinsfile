pipeline{
    agent {label 'deploy'}
    environment{
        staging_server="172.31.0.230"
    }
    stages{
        stage('Deploy to Remote'){
            steps{
              sh 'scp -r /var/lib/jenkins/workspace/* ubuntu@172.31.0.230:/home/ubuntu/'
              
              }
        }
    }
}
