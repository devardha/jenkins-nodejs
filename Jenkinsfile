pipeline {
	agent any
		
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