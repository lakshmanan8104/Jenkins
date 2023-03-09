pipeline{
    agent any
    environment{
        staging_server="172.31.1.171"
    }
    stages{
        stage('Deploy to Remote'){
            steps{
              sh 'sudo scp -r ${WORKSPACE}/* ubuntu@172.31.1.171:/home/destination/'
              }
        }
    }
}
