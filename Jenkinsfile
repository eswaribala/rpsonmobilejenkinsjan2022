pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'Rocking'
            timeout(time: 10)
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