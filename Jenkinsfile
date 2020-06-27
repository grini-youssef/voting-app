pipeline {
  agent {
    node {
      label 'ubuntu-1604-aufs-stable'
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