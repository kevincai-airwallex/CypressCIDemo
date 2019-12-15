pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''echo "Running build ${BUILD_ID} on ${JENKINS_URL}"
sh "npm install -g yarn"
sh "yarn install"'''
      }
    }
  }
}