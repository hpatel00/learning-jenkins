pipeline {
  agent any

  stages {
    stage('One') {
      steps {
        addShortText background: '', borderColor: '', color: '', link: '', text: 'One'
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

