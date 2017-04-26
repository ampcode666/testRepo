pipeline {
  agent any
  stages {
    stage('First') {
      steps {
        parallel(
          "First": {
            echo 'Test'
            
          },
          "analyze": {
            waitForQualityGate()
            
          }
        )
      }
    }
    stage('ha') {
      steps {
        echo 'haha'
      }
    }
  }
}