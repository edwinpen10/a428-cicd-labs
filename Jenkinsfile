node {
    stage('Build'){
         agent {
            docker {
                image 'node:16-buster-slim' 
                args '-p 3000:3000' 
            }
        }
        sh "npm install" 
    }

}