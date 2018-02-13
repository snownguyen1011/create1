pipeline {
  agent any
  
  stages {
    stage('SCM-CHECKOUT') { 
          steps {
            script {
            try { 
            echo 'Fetching CICD source code'
               git(url: 'https://github.com/snownguyen1011/CICD.git', branch: 'master', credentialsId: 'ravi', poll: true, changelog: true)
            echo 'Ready to Build'
          }
            catch(e)
            {
              echo 'SCM - Checkout failed'
            }
            }
        }
  }
}
}
        

