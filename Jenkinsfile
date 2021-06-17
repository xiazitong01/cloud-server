pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'https://github.com/xiazitong01/cloud-server.git', branch: 'master')
        sh '''cd $WORKSPACE
mvn clean package'''
      }
    }

  }
}