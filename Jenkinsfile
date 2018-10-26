pipeline {
  agent any
  stages {
    stage('Build User Service') {
      parallel {
        stage('Build User Service') {
          steps {
            echo 'Started building user service'
          }
        }
        stage('Build Frontend') {
          steps {
            echo 'Starting to build Frontend'
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