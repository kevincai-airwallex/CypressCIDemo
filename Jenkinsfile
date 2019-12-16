pipeline {
  agent any
  stages {
    stage('Dependencies') {
      steps {
        sh 'npm i'
        sh 'npm install start-server-and-test'
      }
    }
    stage('Build') {
      steps {
        echo 'build process'
      }
    }
    stage('e2e Tests') {
      steps {
        sh 'npm run test'
      }
    }
  }
  tools {
    nodejs 'NodeJS 13'
  }
  environment {
    CHROME_BIN = '/bin/google-chrome'
  }
  post {
    // shutdown the server running in the background
    always {
      echo 'Stopping local server'
      sh 'Ctrl-c'
    }
  }
}
