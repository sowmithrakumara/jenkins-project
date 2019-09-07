pipeline {
  agent any
  stages {
    stage('Stage 1') {
      parallel {
        stage('Step1') {
          steps {
            echo 'Step 1 executing'
          }
        }
        stage('Step2') {
          steps {
            echo 'Step 2 executing'
          }
        }
      }
    }
    stage('Stage 2') {
      steps {
        sleep 5
      }
    }
  }
}
