pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'Steeping into compilation'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            bat 'mvn -v'
          }
        }

        stage('functionaltest') {
          steps {
            bat 'java -version'
          }
        }

        stage('integrationtest') {
          steps {
            echo 'integration test'
          }
        }

      }
    }

  }
}