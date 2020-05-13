pipeline {
  agent any
  stages {
    stage('Hello') {
      agent any
      steps {
        echo 'Hello World'
      }
    }

    stage('compile') {
      steps {
        sh '''ls
echo "............"
whoami
#javac HelloWorld.java
echo "............"
#java HelloWorld
'''
      }
    }

  }
}