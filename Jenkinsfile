pipeline {
  agent any
  stages {
    stage('Hello') {
      agent {
        docker {
          image 'ubuntu'
        }

      }
      steps {
        echo 'Hello World'
      }
    }

    stage('compile') {
      steps {
        sh '''ls
echo "............"
javac HelloWorld.java
echo "............"
java HelloWorld
'''
      }
    }

  }
}