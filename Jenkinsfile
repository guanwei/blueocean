pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'I am building some code!'
      }
    }
    stage('Test') {
      steps {
        parallel(
          "Unit Tests": {
            echo 'Unit Tests Are Awesome!'
            
          },
          "Integration Tests": {
            echo 'Integration Tests Are Awesome!'
            
          },
          "Smoke Tests": {
            echo 'Where There is Smoke there is Fire!!!'
            
          },
          "where am i": {
            echo 'hello i am here'
            
          }
        )
      }
    }
    stage('Deploy') {
      steps {
        echo 'Ship It!'
      }
    }
  }
}