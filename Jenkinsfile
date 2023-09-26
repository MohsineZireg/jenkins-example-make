pipeline {
  agent { docker { image 'alpine3.18' } }
  stages {
    stage('Prepare Environment') {
            steps {
                // Install 'make' using the 'apk' package manager
                sh 'apk update && apk add make'
            }
    stage('verify make is installed') {
      steps {
        sh 'make --version'
      }
    }
    stage('run make') {
      steps {
        sh 'make'
      }
    }
  }
}
