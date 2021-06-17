pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git 'https://github.com/xiazitong01/cloud-server.git'
        sh 'mvn clean package'
      }
    }
  }
}
