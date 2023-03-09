pipeline{
    agent any
    environment{
        staging_server="172.31.1.171"
    }
    stages{
        stage('Deploy to Remote'){
            steps{
              sh ' scp -r ${WORKSPACE}/* ubuntu@${staging_server}:/home/destination/'
              }
        }
    }
}
