pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'Steeping into compilation'
      }
    }

    stage('test') {
      steps {
        bat 'mvn -v'
      }
    }

  }
}