// pipeline {
//   agent any
//
//     options {
//         ansiColor('xterm')
//     }
//
//   triggers {
//     pollSCM('*/1 * * * *')
//   }
//
//   tools {
//     maven 'maven-3.6.3'
//   }
//
//   environment {
//     ENV_URL = "pipeline.google.com"
//     SSH_CREDS = credentials("SSH")
//   }
//
//   parameters {
//               string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
//               text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')
//               booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')
//               choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')
//               password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
//           }
//
//   stages {
//
//     stage('One') {
//       when {
//         environment name: "CHOICE", value: 'One'
//       }
//       environment {
//         ENV_URL = "stage.google.com"
//       }
//       steps {
//         addShortText background: '', borderColor: '', color: '', link: '', text: 'One'
//         echo "One"
//         sh '''
//             echo ENV_URL = ${ENV_URL}
//             echo -e "\\e[31mHello"
//             env
//         '''
//       }
//     }
//
//     stage('Two') {
//       when {
//               environment name: "CHOICE", value: 'Two'
//       }
//
//       input {
//           message "Should we continue?"
//           ok "Yes, we should."
//           submitter "alice,bob"
//           parameters {
//               string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
//           }
//       }
//
//       steps {
//         sh '''
//             echo Hello1
//             echo Hello2
//             echo ENV_URL = ${ENV_URL}
//             mvn --version
//         '''
//       }
//     }
//   }
// }
//

pipeline {
  agent any
  stages {

    stage('One') {
        steps {
            sh 'sleep 10'
        }
    }

    stage('Two') {
        steps {
            sh 'sleep 10'
        }
    }

    stage('Three') {
        steps {
            sh 'sleep 10'
        }
    }
  }
 }