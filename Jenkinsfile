pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'Rocking'
          }
        }

        stage('install') {
          steps {
            sh 'npm install'
          }
        }

      }
    }

  }
}