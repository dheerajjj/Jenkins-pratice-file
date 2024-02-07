@Library('my-shared-library') _
pipeline {
  agent any

  stages {
    stage('hello') {
      steps {
        helloWorld()
      }
    }
    stage('Build') {
      steps {
        echo 'Building pipeline now'
      }
    }
  }  
  post {
    always {
      echo 'This will always execute after build'
    }
    success {
      echo 'Build successful'
    }
    failure {
      echo 'Build failed'
    }  
  }
}
