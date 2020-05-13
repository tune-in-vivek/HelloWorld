pipeline {
  agent any
  stages {
    stage('Hello') {
      agent any
      steps {
        sh 'hostname'
      }
    }

    stage('compile') {
      agent {
        docker {
          image 'ubuntu'
        }

      }
      steps {
        sh 'hostname'
      }
    }

  }
}