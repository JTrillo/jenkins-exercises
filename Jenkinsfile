pipeline {
  agent any

  stages {
    stage('Compile') {
      steps {
        echo "Compiling project"
        sh '''
          chmod +x gradlew
          ./gradlew compileJava
        '''
      }
    }
    stage('Unit Tests') {
      steps {
        echo "Running unit tests"
        sh './gradlew test'
      }
    }
  }
}