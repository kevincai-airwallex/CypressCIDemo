pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''echo "Running build ${BUILD_ID} on ${JENKINS_URL}"
echo "${PATH}"
NODEJS_HOME = "${tool node7}"
env.PATH="${env.NODEJS_HOME}:${env.PATH}"
echo ${env.PATH}
sh \'node -version\''''
      }
    }
  }
}