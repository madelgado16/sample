pipeline {
  agent any
  stages {
    stage('install') {
      steps {
        powershell 'npm install'
      }
    }
    stage('Build') {
      steps {
        powershell 'npm run build'
      }
    }
    stage('Test') {
      steps {
        powershell 'npm test'
      }
    }
    stage('approve') {
      steps {
        input(message: '¿se aprueba?', submitter: 'moi')
      }
    }
    stage('Deploy') {
      steps {
        echo 'Succesful'
      }
    }
  }
}