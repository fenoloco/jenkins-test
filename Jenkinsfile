pipeline {
  agent any
  stages {
    stage('message') {
      steps {
        echo 'Do you want to deploy?'
        input(message: 'Do you want to Deploy?', id: '1', ok: '1', submitter: '2', submitterParameter: '3')
      }
    }
  }
}