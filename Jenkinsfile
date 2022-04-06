pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        echo 'Checking out code'
      }
    }

    stage('Build') {
      steps {
        echo 'Building code'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing code'
          }
        }

        stage('MoreTests') {
          steps {
            echo 'Testing More Code'
          }
        }

      }
    }

  }
}