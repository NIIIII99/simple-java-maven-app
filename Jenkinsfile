pipeline {
  agent none
  stages {
    stage('Build') {
      steps {
        echo '"Build"'
        sh 'mvn -B -DskipTests clean package'
      }
    }
  }
}