pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'echo "build"'
          }
        }
        stage('Build2') {
          steps {
            sh 'echo "build 2"'
          }
        }
      }
    }
    stage('Test') {
      steps {
        sh 'echo "test"'
      }
    }
  }
  environment {
    name = 'fred flintstone'
  }
}