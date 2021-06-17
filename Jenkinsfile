pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'https://github.com/xiazitong01/cloud-server.git', branch: 'master')
        bat 'mvn clean package'
      }
    }

    stage('test') {
      steps {
        bat 'mvn clean test'
      }
    }

    stage('deliver') {
      steps {
        sh './deliver.sh'
        input 'deliver Done'
      }
    }

  }
}