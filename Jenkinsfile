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
  }
}