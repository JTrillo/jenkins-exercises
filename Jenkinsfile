pipeline {
  agent any

  stages {
    stage('Compile') {
      steps {
        sh 'gradlew compileJava'
      }
    }
    stage('Unit Tests') {
      steps {
        sh 'gradlew test'
      }
    }
  }
}