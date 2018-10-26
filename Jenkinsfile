pipeline {
  agent any
  stages {
    stage('Build User Service') {
      parallel {
        stage('Build User Service') {
          steps {
            echo 'Started building user service'
            dir(path: 'User-Service') {
              sh 'docker image build -t userservice:1.1-$BUILD_ID .'
            }

          }
        }
        stage('Build Frontend') {
          steps {
            echo 'Starting to build Frontend'
            sh 'docker image build -t frontend:1.1-$BUILD_ID Front-End'
          }
        }
      }
    }
    stage('Build Posts Service') {
      steps {
        echo 'Starting to build posts service'
      }
    }
  }
}
