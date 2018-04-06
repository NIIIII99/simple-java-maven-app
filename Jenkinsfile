pipeline {
  agent none
  stages {
    stage('Build') {
      steps {
        echo '"Build"'
      }
    }
    stage('Test') {
      parallel {
        stage('JUnit') {
          steps {
            echo 'JUnit'
          }
        }
        stage('DBUnit') {
          steps {
            echo 'DBUnit'
          }
        }
      }
    }
    stage('Browser Tests') {
      parallel {
        stage('Firefox') {
          steps {
            echo 'Firefox'
          }
        }
        stage('Edge') {
          steps {
            echo 'Edge'
          }
        }
        stage('Safari') {
          steps {
            echo 'Safari'
          }
        }
        stage('Chrome') {
          steps {
            echo 'Chrome'
          }
        }
      }
    }
    stage('Dev') {
      steps {
        echo 'Dev'
      }
    }
    stage('Staging') {
      steps {
        echo 'Staging'
      }
    }
    stage('Production') {
      steps {
        echo 'Production'
      }
    }
  }
}