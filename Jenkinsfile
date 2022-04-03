pipeline {
  agent any

  stages {
    stage('One') {
      steps {
        echo "One"
      }
    }

    stage('Two') {
      steps {
        sh '''
            echo Hello1
            echo Hello2
        '''
      }
    }
  }
}

