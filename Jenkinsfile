pipeline {
  agent any
  stages {
    stage('SCM-CHECKOUT') {
      parallel {
        stage('Start') {
          steps {
            echo 'Build Started .....'
          }
        }
        stage('Git ') {
          steps {
            git(url: 'https://github.com/snownguyen1011/CICD.git', branch: 'master', credentialsId: 'ravi', poll: true, changelog: true)
          }
        }
        stage('') {
          steps {
            findFiles(glob: '{project-name}')
          }
        }
      }
    }
  }
}