pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''echo "Running build ${BUILD_ID} on ${JENKINS_URL}"
export PATH = ${PATH}
sh \'npm install\''''
      }
    }
  }
}