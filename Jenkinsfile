pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/gangiknol/helloworld.git', branch: 'master', poll: true)
      }
    }

    stage('build') {
      steps {
        sh 'mvn clean package'
      }
    }

    stage('testing') {
      steps {
        sh 'echo test--master'
      }
    }

  }
}