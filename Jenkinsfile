pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
        sh 'npm start'
        sh 'serve -s build'
            }
        }
  environment {
    CI = 'true'
  }
}
