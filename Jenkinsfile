pipeline {
  agent any
  stages {
    stage('DEv') {
      steps {
        echo 'dev'
      }
    }

    stage('Qa') {
      steps {
        echo 'qa'
      }
    }

    stage('UI testing') {
      parallel {
        stage('UI testing') {
          steps {
            echo 'Ui'
          }
        }

        stage('API') {
          steps {
            echo 'api'
          }
        }

        stage('DB') {
          steps {
            echo 'Db'
          }
        }

      }
    }

    stage('QA Prod') {
      steps {
        echo 'prod'
      }
    }

  }
}