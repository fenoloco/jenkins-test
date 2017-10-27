pipeline {
  agent any
  stages {
    stage('Ask to deploy') {
      agent any
      steps {
        input(message: 'Do you want to Deploy?', id: 'deploy_enable', ok: 'Yes', submitter: '1')
      }
    }
    stage('Print User Option') {
      steps {
        echo '${deploy_enable}'
      }
    }
  }
}