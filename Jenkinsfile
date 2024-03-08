pipeline {
  agent any
  stages {
    stage('Build') { 
      steps {
        build 'PES2UG21CS569_TanishaDas-1'
        sh 'g++ main.cpp -o output'
      }
    }
    stage('Test') { 
      steps {
        sh './o'
      }
    }
      
   stage('Deploy') {  
      steps {
        echo 'deploy'
      }
    }
  }
  post{
    failure{
      error 'Pipeline failed'
    }
  }
}

