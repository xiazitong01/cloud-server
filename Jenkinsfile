pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        sh 'mvn clean compile'
      }
    }

    stage('package') {
      steps {
        sh 'mvn clean package'
      }
    }

    stage('install') {
      steps {
        sh 'mvn clean install'
      }
    }

    stage('test') {
      steps {
        sh 'mvn clean test'
      }
    }

  }
}