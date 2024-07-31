pipeline {
	agent any 	
	stages {
		stage('Checkout') {
			steps {
				echo 'Checkout completed in feature2'
			}
		}
		stage('Static-test') {
			steps {
				echo 'Running static tests on code in feature2'
			}
		}
		stage('Build') {
			steps {
				sh 'echo "Building the code in feature2"'
			}
		}
		stage('Deploy') {
		    when {
                branch 'feature2'
            }
			steps {
				echo 'Deploying into environment in feature2'
			}
		}
	}
}
