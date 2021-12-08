pipeline {
  agent any
  tools {
    nodejs 'node-17.2.0'
  }

  options {
    timeout(time: 2, unit: 'MINUTES')
  }

  stages {
    stage('Install dependencies') {
      steps {
        sh 'yarn'
      }
    }
    stage('Run tests') {
      steps {
        sh 'yarn test'
      }
    }
  }
}