pipeline {
  agent any
  stages {
    stage('builed') {
      parallel {
        stage('Server') {
          steps {
            sh 'echo "builed"'
          }
        }

        stage('client') {
          steps {
            sh 'echo "this is client"'
          }
        }

        stage('client1') {
          steps {
            sh 'echo "client1 success"'
          }
        }

      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            sh 'echo "test success"'
          }
        }

        stage('testclient') {
          steps {
            sh 'echo "success client"'
          }
        }

        stage('client2') {
          steps {
            sh 'echo "client 2 success"'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        sh 'echo "deploy success"'
      }
    }

  }
}