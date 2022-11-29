pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/ozgurkk/curriculum-app', branch: 'dev')
      }
    }

    stage('Log') {
      parallel {
        stage('Log') {
          steps {
            sh 'ls -lah'
          }
        }

        stage('FrontEnd Unit Test') {
          steps {
            sh 'cd curriculum-front && npm install --save-dev vue-jest && npm run test:unit'
          }
        }

      }
    }

  }
}