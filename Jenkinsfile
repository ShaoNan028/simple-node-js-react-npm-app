pipeline {
    agent {
        docker {
            image 'node:16-alpine' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'nvm use 16'
                sh 'npm install' 
            }
        }
    }
}