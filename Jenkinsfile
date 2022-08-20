pipeline {
	agent any

	tools { nodejs 'NodeJS' }

		
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
				sh "ssh dev@${env.SSH_HOST} ls"
			}
		}
	}
}