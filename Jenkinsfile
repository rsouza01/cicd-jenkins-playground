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
  agent {
      docker { image 'node:7-alpine' }
  }
  stages {
    stage("Prepare environment") {
      sh "echo Build Type = ${BUILD_TYPE}"
    }
    stage("Build") {
      sh "echo Done"
    }
    stage('Test') {
        steps {
            sh 'node --version'
        }
    }
  }
}
