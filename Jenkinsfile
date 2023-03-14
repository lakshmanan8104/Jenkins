pipeline{
    agent any
    environment{
        staging_server="172.31.32.229"
    }
    stages{
        stage('Deploy to Remote'){
            steps{
              sh ' scp -r ${WORKSPACE}/* jenkins@${staging_server}:/home/ubuntu/'
              }
        }
    }
}
