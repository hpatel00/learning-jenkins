pipeline {
  agent any

  environment {
    ENV_URL = "pipeline.google.com"
  }

  stages {

    stage('One') {
      environment {
        ENV_URL = "stage.google.com"
      }
      steps {
        addShortText background: '', borderColor: '', color: '', link: '', text: 'One'
        echo "One"
        sh 'echo ENV_URL = ${ENV_URL}'
      }
    }

    stage('Two') {
      steps {
        sh '''
            echo Hello1
            echo Hello2
            echo ENV_URL = ${ENV_URL}
        '''
      }
    }
  }
}

