pipeline {
  agent any
  environment {
    SERVER_IP_1 = "192.168.43.222"
    SERVER_DEPLOY_DIR = "/home/lunix/reactjs/src"
  }
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
        sh 'npm start'
        sh 'serve -s build'
        archiveArtifacts 'src/app.js'
      }
    }

  }
}
