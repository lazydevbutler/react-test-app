pipeline {
  agent any
  stages {
    stage('Initialise') {
      steps {
        bat 'yarn install'
      }
    }

    stage('Test') {
      steps {
        bat 'yarn test'
      }
    }

    stage('Publish') {
      steps {
        bat 'yarn build'
        bat 'del /f/s/q C:\\website-react\\*'
        bat 'rmdir /s/q C:\\website-react\\*'
      }
    }

  }
}