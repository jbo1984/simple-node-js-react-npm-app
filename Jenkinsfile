pipeline {
  
    stages {
        stage('Build') {
              agent {
        docker { image 'node:14-alpine' }
    }
            steps {
              echo 'Start build'
                sh 'node --version'
              sh 'npm install'
              sh 'npm run build'
            }
        }
    }
}
