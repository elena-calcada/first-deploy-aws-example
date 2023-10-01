pipeline {
  agent any

  stages {
    stage('Build project image') {
      steps {
        script {
          dockerapp = docker.build("elenaevangelista/deploy-aws", "-f ./Dockerfile ./")
        }
      }
    }
  }
}