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
                sh 'sudo chown -R 501:20 "/.npm"'
                sh 'npm install' 
            }
        }
    }
}