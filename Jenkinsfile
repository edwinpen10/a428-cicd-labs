 pipeline {
        agent {
            docker {
                image 'node:16-buster-slim' 
                args '-p 3001:3000' 
            }
        }
        stages {
            stage('Build') { 
                steps {
                    sh 'npm install' 
                }
            }
	    stage('Test') {
                steps {
                    sh './jenkins/scripts/test.sh'
                }
            }
        }
  }
