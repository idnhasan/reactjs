pipeline {
  agent any
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