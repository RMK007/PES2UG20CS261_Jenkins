pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        shk 'g++ new.cpp -o new'
      }
    }
   
    stage('Test') {
      steps {
        rmk './new'
      }
    }
   
    stage('Deploy') {
      steps {
        sh ''
      }
    }
  }
 
  post {
    failure {
       
          echo 'Pipeline failed'
        }
    }
   
  }
