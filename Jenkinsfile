pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building'
      }
    }
    stage('Test') {
      steps {
        echo 'Testing'
      }
    }
    stage('UAT') {
      steps {
        echo 'Running UAT'
        input(message: 'Are you happy', id: 'HappyReq', ok: 'Yes')
      }
    }
    stage('Prod') {
      steps {
        echo 'Running live instance'
      }
    }
  }
}