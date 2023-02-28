pipeline{
    agent any
    environment{
        staging_server="GITHUB-Runner.shrigroupidc.com"
    }
    stages{
        stage('Deploy to Remote'){
            steps{
              sh ' scp -r ${WORKSPACE}/* root@${staging_server}:/var/mbaquatech/'
              }
        }
    }
}
