pipeline {
  agent any
  stages {
    stage('Start Build') {
      parallel {
        stage('Start Build') {
          steps {
            echo 'Build Started...'
          }
        }

        stage('Check Tools Version') {
          steps {
            sh 'git --version; java -version; mvn --version'
          }
        }

      }
    }

  }
}