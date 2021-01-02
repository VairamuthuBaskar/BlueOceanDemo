pipeline {
  agent any
  stages {
    stage('Development Build') {
      steps {
        echo 'Development'
      }
    }

    stage('Smoke Test') {
      steps {
        echo 'Smoke Test Performed'
      }
    }

    stage('Deploy in QA') {
      steps {
        echo 'Deployed in QA'
      }
    }

    stage('Integration Test') {
      parallel {
        stage('Integration Test') {
          steps {
            echo 'Integration Test Done'
          }
        }

        stage('Performance Test') {
          steps {
            echo 'Performance Test Done'
          }
        }

        stage('UI Test') {
          steps {
            echo 'UI Test Done'
          }
        }

      }
    }

  }
}