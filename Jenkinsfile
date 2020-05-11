pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
        sh 'npm start'
        sh 'npm install -g serve'
        sh 'serve -s build'
      }
    }

  }
  environment {
    CI = 'true'
  }
}