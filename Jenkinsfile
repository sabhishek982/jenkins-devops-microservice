pipeline {
	agent { docker { image 'maven:latest'} } //Using docker image as pipeline agent
	stages {
		stage('Build') {
			steps {
				sh 'mvn --version'
				echo "Build"
			}
		}
		stage('Test') {
			steps {
				echo "Test"
			}
		}
		stage('Integration Test') {
			steps {
				echo "Integration Test"
			}
		}
	} 
	post {
		always {
			echo ' I run always'
		}
		success {
			echo 'I run on success'
		}
		failure {
			echo 'I run on failure'
		}
	}
}
