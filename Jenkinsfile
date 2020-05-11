pipeline {
  agent any
  stages {
    stage('Git') {
      steps {
        git 'https://github.com/idnhasan/reactjs.git'
      }
    }

    stage('Build') {
      steps {
        sh 'npm install'
      }
    }

    stage('after build') {
      steps {
        sh 'npm install -g serve'
        sh 'serve -s build'
      }
    }

    stage('Test') {
      steps {
        sh 'node test'
      }
    }

  }
  tools {
    nodejs 'node'
  }
}