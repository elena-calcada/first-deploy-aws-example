pipeline {
  agent any

  stages {
    stage('Build project image') {
      steps {
        script {
          dockerapp = docker.build("elenaevangelista/deploy-aws:${env.BUILD_ID}", "-f ./Dockerfile ./")
        }
      }
    }
  }
}