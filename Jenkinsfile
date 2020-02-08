pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'This is the Build Stage, changed by tyao'
          }
        }

        stage('Build2') {
          steps {
            echo 'This is Build2 Message'
          }
        }

      }
    }

    stage('Test') {
      steps {
        echo 'This is the Testing Stage'
      }
    }

    stage('Deploy') {
      steps {
        echo 'This is the Deploy Stage'
      }
    }

  }
  environment {
    env = 'windows'
  }
}