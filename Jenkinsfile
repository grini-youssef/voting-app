pipeline {
  agent {
    node {
      label 'master'
    }
  }
  stages {
    stage('Build result') {
      steps {
        sh 'docker build -t grini/result ./result'
      }
    } 
    stage('Build vote') {
      steps {
        sh 'docker build -t grini/vote ./vote'
      }
    }
    stage('Build worker') {
      steps {
        sh 'docker build -t grini/worker ./worker'
      }
    }
  }
}
