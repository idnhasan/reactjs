pipeline {
  agent any
    
  tools {nodejs "node"}
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/idnhasan/reactjs.git'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
         sh '<<Build Command>>'
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
}
