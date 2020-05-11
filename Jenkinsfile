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
    stage('Archive artifact') {
            steps {
                archiveArtifacts 'src/app.js'
            onlyIfSuccessful: 'true'
            }
        }
    }
}
