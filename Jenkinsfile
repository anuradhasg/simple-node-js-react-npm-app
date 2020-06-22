pipeline {
    agent {
        "/c/Program Files/Docker Toolbox/docker" {
            image 'node:6-alpine'
            args '-p 3000:3000'
        }
    }
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }
        
    
    }
}
