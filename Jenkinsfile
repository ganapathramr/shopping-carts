pipeline {
  agent any
   tools{
       maven 'maven'
    }
  stages {
    stage('build-the-app') {
      steps {
        echo 'This is the build step'
        sh 'mvn compile'
      }
    }

  }
}
