pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''echo "Running build ${BUILD_ID} on ${JENKINS_URL}"
echo "${PATH}"
checkout scm
sh "yarn"'''
      }
    }
  }
}