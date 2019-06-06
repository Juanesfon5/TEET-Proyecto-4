pipeline {
  agent any
  stages {
    stage('Change Dir') {
      steps {
        dir(path: './teetproyecto4/src')
      }
    }
    stage('Dependecias ') {
      steps {
        sh 'npm install -g'
      }
    }
  }
}