pipeline {
  agent any
  stages {
    stage('stage 1') {
      parallel {
        stage('stage 1') {
          steps {
            sh 'echo "stage 1"'
          }
        }

        stage('parallel 1.1') {
          steps {
            sh '''sleep 10
echo "parallel stage 1.1"'''
          }
        }

      }
    }

    stage('stage 2') {
      parallel {
        stage('stage 2') {
          steps {
            sh 'echo "stage 2"'
          }
        }

        stage('parallel 2.2') {
          steps {
            sh '''sleep 10
echo "parallel stage 2.1"'''
          }
        }

      }
    }

  }
}