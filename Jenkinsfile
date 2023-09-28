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
        sh 'npm cache clear --force'
      }
    }

    stage('testing frontend') {
      steps {
        sh 'cd curriculum-front && npm i && npm run test:unit'
      }
    }

  }
}