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
	 		
    
    
	stage('Test') {
            steps {
                sh './jenkins/scripts/test.sh'
            }
        }
    stage('Deploy') {
			steps {
                sh './jenkins/scripts/deliver.sh' 
                input message: 'Finished using the web site? (Click "Proceed" to continue)' 
                sh './jenkins/scripts/kill.sh' 
            }
        }
		}
	
}
