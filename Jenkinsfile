pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/ozgurkk/curriculum-app', branch: 'dev')
      }
    }

    stage('error') {
      steps {
        sh 'ls -lah'
      }
    }

  }
}