pipeline {
  agent any

  stages {
    stage('hello') {
      steps {
        echo 'Hello DevOps Engineer'
      }
    }
    stage('Build') {
      steps {
        echo 'Building pipeline now'
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
