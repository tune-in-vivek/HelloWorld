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
          image 'openjdk'
        }

      }
      steps {
        sh '''ls
javac HelloWorld.java
java HelloWorld'''
        archiveArtifacts 'HelloWorld.class'
      }
    }

  }
}