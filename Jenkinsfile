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

    stage('package-the-app') {
      steps {
        sh 'mvn package -DskipTests'
      }
    }

    stage('archive') {
      steps {
        archiveArtifacts '**/target/*.jar'
      }
    }

  }
  tools {
    maven 'maven'
  }
}