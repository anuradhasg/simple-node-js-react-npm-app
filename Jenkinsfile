pipeline {
    agent any
        
    
    environment {
        CI = 'true'
    }
    stages {
        stage('Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/anuradhasg/simple-node-js-react-npm-app.git'
            }
        }
        
    
    }
}
