pipeline {
  agent any

  stages {
    stage('Run in Podman container') {
      steps {
        sh '''
          podman pull node:16-alpine
          podman run --rm node:16-alpine node --version
        '''
      }
    }
  }
}
