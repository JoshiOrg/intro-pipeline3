pipeline {
  agent any
  stages {
    stage('Say Hello') {
      steps {
        echo 'Hello!'
      }
    }
    stage('') {
      steps {
        sh '''pipeline {
   agent any
   stages {
      stage(\'Say Hello\') {
         steps {
            echo \'Hello World!\'   
            sh \'java -version\'
         }
      }
   }
}
'''
        }
      }
    }
  }