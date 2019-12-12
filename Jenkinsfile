pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build done'
        echo 'unit test done'
      }
    }
    stage('Test') {
      parallel {
        stage('UI Test') {
          steps {
            echo 'UI test done'
          }
        }
        stage('backend test') {
          steps {
            echo 'backend test done'
          }
        }
      }
    }
    stage('Deploy to staging ') {
      steps {
        echo 'Deploy done!'
      }
    }
  }
}