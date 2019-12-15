pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''
echo "Running build ${env.BUILD_ID} on ${env.JENKINS_URL}"
sh \'yarn debug\'
'''
      }
    }
  }
}