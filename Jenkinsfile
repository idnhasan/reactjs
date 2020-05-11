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
  stage('Test') { 
            steps {
                sh './src/app.js' 
            }
        }
  environment {
    CI = 'true'
  }
}
