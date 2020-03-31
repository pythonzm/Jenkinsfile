pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'echo "$NAME"'
          }
        }

        stage('Build2') {
          environment {
            hello = 'world'
          }
          steps {
            echo '"$hello"'
          }
        }

      }
    }

  }
  environment {
    NAME = 'zm'
  }
}