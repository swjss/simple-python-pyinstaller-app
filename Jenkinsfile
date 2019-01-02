pipeline {
  agent {
    node {
      label 'aaaa'
    }

  }
  stages {
    stage('1') {
      parallel {
        stage('1') {
          steps {
            sh 'echo "hello world" | grep "hello"'
          }
        }
        stage('sss') {
          steps {
            echo 'sssssss'
          }
        }
      }
    }
    stage('2') {
      parallel {
        stage('2') {
          steps {
            sh 'who && pwd'
          }
        }
        stage('3') {
          steps {
            sleep 5
          }
        }
      }
    }
  }
  environment {
    swj = '1'
  }
}