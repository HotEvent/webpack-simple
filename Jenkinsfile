pipeline {
  agent any
  stages {
    stage('Example') {
      steps {
        parallel(
          "Example": {
            sh 'npm run build'
            
          },
          "\u90E8\u7F72": {
            sh 'npm run build'
            
          }
        )
      }
    }
    stage('test') {
      steps {
        sh 'npm -v'
      }
    }
  }
  tools {
    nodejs 'node6.10.0'
  }
}