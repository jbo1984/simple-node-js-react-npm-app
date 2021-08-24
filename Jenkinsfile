pipeline {
    agent {
        docker { image 'node:14-alpine' }
    }
    stages {
        stage('Build') {
            steps {
              echo 'Start build'
                sh 'node --version'
              sh 'npm install'
              sh 'npm run build'
            }
        }
    }
}
