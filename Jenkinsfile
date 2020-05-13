pipeline {
  agent any
  stages {
    stage('Hello') {
      agent any
      steps {
        sh 'host'
      }
    }

    stage('compile') {
      agent {
        docker {
          image 'ubuntu'
        }

      }
      steps {
        sh 'host'
      }
    }

  }
}