pipeline {
  agent any
  stages {
    stage('build-the-app') {
      steps {
        echo 'This is the build step'
        sh 'mvn compile'
      }
    }

    stage('test-the-app') {
      steps {
        sh 'mvn test'
      }
    }

  }
  tools {
    maven 'maven'
  }
}