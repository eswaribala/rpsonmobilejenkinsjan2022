pipeline {
  agent any
  stages {
    stage('deploy') {
      parallel {
        stage('deploy') {
          steps {
            echo 'Deployment Successful'
          }
        }

        stage('monitoring') {
          steps {
            bat 'mvn -v'
          }
        }

      }
    }

  }
}