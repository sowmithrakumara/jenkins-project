pipeline {
  agent any
  stages {
    stage('Stage1') {
      parallel {
        stage('Stage1') {
          steps {
            echo 'Hello Pipeline-1'
            build(job: 'HP1', quietPeriod: 2)
          }
        }
        stage('Stage2') {
          steps {
            build(job: 'Stage2', quietPeriod: 1)
            build(job: 'Stage3', quietPeriod: 3)
          }
        }
      }
    }
  }
}