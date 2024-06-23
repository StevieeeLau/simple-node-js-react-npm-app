pipeline {
    agent any
	tools {
        nodejs 'NodeJS 22' // This should match the name of the NodeJS installation in Jenkins configuration
    }
    stages {
        stage('Build') { 
            steps {
				script {
                    env.PATH = "${tool name: 'NodeJS 22'}/bin:${env.PATH}"
                }
				sh 'node -v'
                sh 'npm -v'
                sh 'npm install' 
            }
        }
    }
}