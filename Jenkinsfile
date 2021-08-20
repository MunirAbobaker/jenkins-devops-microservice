
// declarative 
pipeline {
	// agent any 

	agent { docker { image 'maven:3.6.3'}}
	stages {
		stage ("Build"){
			steps {
				echo "Build"
				sh "mvn --version"
			}
		}
		stage ("Test"){
			steps {
				echo "Test"
			}
		}
		stage ("Integration Test"){
			steps {
				echo "Integration Test"
			}
		}
	} 
	
	post { // define what to after success or failler
		always { 
			echo "I run always ok"
		}
		success {
			echo "I run when successfully"
		}
		failure {
			echo "I run when you fail"

		}
	}
}