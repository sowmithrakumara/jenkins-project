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
	        stage('Stage 2') {
	          steps {
	            build(job: 'hp1', quietPeriod: 2)
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

