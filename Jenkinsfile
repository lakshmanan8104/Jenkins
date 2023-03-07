pipeline{
    agent any
    environment{
        staging_server="172.16.200.30"
    }
    stages{
        stage('Deploy to Remote'){
            steps{
              sh ' scp -r ${WORKSPACE}/* jenkins@${staging_server}:/var/lib/jenkins/'
              }
        }
    }
}
