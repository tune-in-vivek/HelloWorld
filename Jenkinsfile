pipeline {
  agent any
  stages {
    stage('Hello') {
      agent any
      steps {
        sh '''hostname
ls'''
      }
    }

    stage('compile') {
      agent {
        docker {
          image 'ubuntu'
        }

      }
      steps {
        sh '''hostname
ls
javac HelloWorld.java
java HelloWorld'''
      }
    }

  }
}