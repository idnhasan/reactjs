pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
        sh 'npm start'
      }
    }

  }
  environment {
    SERVER_IP_1 = '192.168.43.222'
    SERVER_DEPLOY_DIR = '/home/lunix/reactjs/src'
    DEPLOY = 'npm run deploy'
  }
}