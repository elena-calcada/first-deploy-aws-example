pipeline {
  agent any

  stages {
    stage('Build project image') {
      steps {
        script {
          dockerapp = docker.build("elenaevangelista/first-deploy-aws", "-f ./Dockerfile ./")
        }
      }
    }
  }
}