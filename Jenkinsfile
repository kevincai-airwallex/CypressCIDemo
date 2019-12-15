pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''echo "Running build ${BUILD_ID} on ${JENKINS_URL}"
sh \'apt-get update && apt-get -y install xvfb\''''
      }
    }
  }
}