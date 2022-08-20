pipeline {
	agent any

	tools {
        NodeJS 'node-18.7.0'
    }

		
	stages {
			
		stage('Git') {
			steps {
				git 'https://github.com/devardha/jenkins-nodejs.git'
			}
		}
		
		stage('Build') {
			steps {
				echo 'Installing dependencies'
				sh 'npm install'
			}
		}  
		
				
		stage('Deployment') {
			steps {
				echo 'Deploying application'
			}
		}
	}
}