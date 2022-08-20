pipeline {
	agent any

	tools {
        NodeJS 'NodeJS'
    }

		
	stages {
		stage('Review node and npm installations') {
			steps {
				nodejs(nodeJSInstallationName: 'NodeJS') {
					sh 'npm -v'
					sh 'node -v'
				}
			}
		}
			
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