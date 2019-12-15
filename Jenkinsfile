pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''echo "Running build ${BUILD_ID} on ${JENKINS_URL}"
echo "${PATH}"
sh "node -v"'''
      }
    }
  }
}