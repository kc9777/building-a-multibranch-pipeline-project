pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'echo "Hello world!"'
          }
        }
        stage('build2') {
          steps {
            sleep 5
          }
        }
        stage('build3') {
          steps {
            echo 'bye..bye'
          }
        }
        stage('checkout') {
          steps {
            git 'https://github.com/kc9777/building-a-multibranch-pipeline-project.git'
          }
        }
      }
    }
  }
}