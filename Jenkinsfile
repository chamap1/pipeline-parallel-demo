pipeline {
  agent any
  stages {
    stage('NexB Scan') {
      steps {
        parallel(
          "NexB Scan": {
            sh 'rm -rf .repo'
            
          },
          "SonarQube Analysis": {
            echo 'testing'
            
          }
        )
      }
    }
    stage('Post Actions') {
      steps {
        echo 'cads'
      }
    }
  }
}