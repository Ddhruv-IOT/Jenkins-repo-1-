pipeline {

	agent any

	stages {	

		stage ('SCM') {
			steps {
				echo "git pull my code"
				git 'https://github.com/Ddhruv-IOT/simple-java-maven-app.git'
			}	
		}

		stage ('Deploy') {
			steps {
				echo "Deploy"
				sh 'mvn clean package'
			}	
		}		

		stage ('Test') {
			steps { 
				echo "final test"
			}
		}
	}
}
