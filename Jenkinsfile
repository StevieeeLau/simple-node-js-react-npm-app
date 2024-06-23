pipeline {
    agent any
	tools {
        nodejs 'NodeJS 22' // This should match the name of the NodeJS installation in Jenkins configuration
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
		stage('Test') { 
				steps {
					sh './jenkins/scripts/test.sh' 
				}
		}
    }
}