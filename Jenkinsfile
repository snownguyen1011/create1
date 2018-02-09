pipeline {
  agent any
  stages {
    stage('SCM-CHECKOUT') {
      parallel {
        stage('SCM-CHECKOUT') {
          steps {
            echo 'Build Started .....'
          }
        }
        stage('') {
          steps {
            git(url: 'https://github.com/snownguyen1011/CICD.git', branch: 'master', credentialsId: 'ravi', poll: true, changelog: true)
          }
        }
      }
    }
  }
}