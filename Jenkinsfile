pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        parallel(
          "Build": {
            sh 'go build'
            
          },
          "Log Built": {
            echo 'Built'
            
          }
        )
      }
    }
    stage('Done') {
      steps {
        sleep 5
      }
    }
  }
}