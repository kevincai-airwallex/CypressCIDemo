pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''echo "Running build ${BUILD_ID} on ${JENKINS_URL}"
PATH = /usr/local/bin:${PATH}
echo "${PATH}"
sh \'npm install\''''
      }
    }
  }
}