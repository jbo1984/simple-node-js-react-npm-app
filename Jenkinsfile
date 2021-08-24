pipeline {
    agent {
        docker {
            image 'node:lts-buster-slim' 
            args '-p 3000:3000' 
        }
        
    }
    stages {
         stage('Checkout'){

          checkout scm
       }
        stage('Build') { 
            steps {
                sh 'npm --version'
                sh 'node --version'
                sh 'npm install' 
            }
        }
    }
}
