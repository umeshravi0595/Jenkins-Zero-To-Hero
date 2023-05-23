pipeline {
  agent {
    docker { 
      image 'node:16-alpine' 
  }
}
  tools {
        maven 'apache-maven-3.0.1'
        dockerTool  'docker'
    }
  stages {
    stage('SCM Checkout') {
            steps{
            git 'https://github.com/umeshravi0595/Jenkins-Zero-To-Hero.git'
            }
        }
    stage('TeSt') {
      steps {
        sh 'node --version'
      }
    }
  }
}

