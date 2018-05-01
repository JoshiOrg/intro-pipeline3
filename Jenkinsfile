pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('error') {
      steps {
        echo 'Hello World!'
        sh 'java -version'
      }
    }
  }
}