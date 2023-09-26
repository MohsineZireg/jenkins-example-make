pipeline {
  agent { docker { image 'make-alpine3.18' } }
  stages {
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
