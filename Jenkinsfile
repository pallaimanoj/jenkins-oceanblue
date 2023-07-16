pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        sh '''pwd
date
cal 2024'''
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'this is manoj'
          }
        }

        stage('build para') {
          steps {
            sh 'echo ${BUILD_ID}'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'deploy to test'
      }
    }

  }
}