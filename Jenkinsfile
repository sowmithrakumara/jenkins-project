pipeline {
  agent any
  stages {
    stage('Stage1') {
      parallel {
        stage('Stage1') {
          steps {
            echo 'Stage 1 executing'
          }
        }
        stage('') {
          steps {
            echo 'hello '
          }
        }
      }
    }
    stage('Blue stage1') {
      steps {
        sleep 5
      }
    }
  }
}