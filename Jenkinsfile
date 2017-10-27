pipeline {
  agent any
  stages {
    stage('Ask to deploy') {
      steps {
        input(message: 'Do you want to Deploy?', id: '1', ok: 'Yes', submitter: 'true', submitterParameter: 'deploy_enable')
      }
    }
    stage('Print User Option') {
      steps {
        echo '${deploy_enable}'
      }
    }
  }
}