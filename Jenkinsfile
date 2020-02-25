#!groovy

pipeline {
  environment {
  BUILD_TYPE = 'NIGHTLY'
  CICD_ENV = 'true'
  PLATFORM_NAME = 'platform_name'
  CF_URL = "cloundfroundry.com"
  VAULT_URL = "http://www.vault.com"
  VAULT_SERVICE_NAME = "vault-cicd"
  }
  agent any
  stages {
    stage("Prepare environment") {
      steps{
        sh "echo Build Type = ${BUILD_TYPE}"
      }
    }
    stage("Build") {
      steps{
        sh "echo Done"
      }
    }
    stage('Test') {
        steps {
            sh 'node --version'
        }
    }
  }
}
