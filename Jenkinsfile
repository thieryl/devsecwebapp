pipeline {
  agent {
    node {
      label 'jenkins_mvn_agent'
    }

  }
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

    stage('Build') {
      steps {
        sh 'mvn clean package'
      }
    }

  }
}