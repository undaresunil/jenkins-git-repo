pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Build jenkins repo'
          }
        }

        stage('Build-repo') {
          steps {
            echo 'Build Repository'
          }
        }

      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing Applicstion'
          }
        }

        stage('Test1') {
          steps {
            echo 'Test1 Application'
            echo 'test 2 added here'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy Application'
      }
    }

  }
}