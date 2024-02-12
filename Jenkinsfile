pipeline {
  agent any
  
  stages {
    stage('checkout stage') {
      steps {
        sh 'rm -rf prometheus'
        sh 'https://github.com/sudhasanshi/prometheus.git'
      }
    }
    stage('running playbook') {
      steps {
        sh 'ansible-playbook -i hosts prometheus1.yml'
      }
    }
  }
}
