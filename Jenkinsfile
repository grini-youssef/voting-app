pipeline {
  agent any

  stages {

    stage('Build vote') {
      steps {
        sh 'docker build -t grini-youssef/vote ./vote'
      }
    }
  }
}
