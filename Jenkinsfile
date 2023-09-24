pipeline {
  agent any
  stages {
    stage('checkout code') {
      steps {
        git(url: 'https://github.com/omaraalsaied/curriculum-app', branch: 'dev', credentialsId: 'github')
      }
    }

    stage('listing the dir') {
      steps {
        sh 'ls -la '
      }
    }

  }
}