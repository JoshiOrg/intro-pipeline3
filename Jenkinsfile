pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('error') {
      steps {
        echo "Hello World ${params.Name}!"
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PWD}"
        sh 'java -version'
      }
    }
  }
  environment {
    MY_NAME = 'Mary'
    TEST_USER = credentials('test-user')
  }
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}