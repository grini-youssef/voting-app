pipeline {
  agent {
    node {
      label 'ubuntu-1604-aufs-stable'
    }
  }
  stages {

    stage('Build vote') {
      steps {
        sh 'docker build -t grini-youssef/vote ./vote'
      }
    }
  }
}
