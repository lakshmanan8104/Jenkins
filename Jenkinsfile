pipeline{
    agent any
    environment{
        staging_server="GITHUB-Runner.shrigroupidc.com"
    }
    stages{
        stage('Deploy to Remote'){
            steps{
              sh ' scp -r ${WORKSPACE}/* dcadmin@${staging_server}:/var/mbaquatech/'
              }
        }
    }
}
