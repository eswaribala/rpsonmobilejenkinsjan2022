pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'Rocking'
            timeout(time: 10, activity: true)
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