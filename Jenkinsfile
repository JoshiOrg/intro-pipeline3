pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('error') {
      steps {
        echo "Hello World ${params.Name}!"
        sh 'java -version'
      }
    }
  }
  environment {
    MY_NAME = 'Mary'
  }
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}