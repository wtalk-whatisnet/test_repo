pipeline {
  agent any
  stages {
    stage('run01') {
      steps {
        sh '''hostname
pwd
'''
        sh 'ls -al /tmp/'
      }
    }

    stage('run02') {
      steps {
        sleep 1
      }
    }

    stage('run03') {
      steps {
        sh 'echo $ENV'
      }
    }

  }
  environment {
    ENV = 'dev'
  }
}