pipeline{
	agent {
		docker {image 'maven:3.9-sapmachine-17'}}
	stages{
		stage('Build') {
			steps{
				sh 'mvn --version'
				echo "Build"
			}
		
		}
		// stage('Test') {
		// 	steps{
		// 		echo "Test"
		// 	}
		// }
		// stage('Integration Test') {
		// 	steps{
		// 		echo "Integration Test"
		// 	}
			
		// }
	} 
	post{
		always{
			echo "I am aweasome. I run always"
		}
		success
		{
			echo "Run When I am succesful"
		}
		failure{
			echo "Run When I fail"
		}
	}
}
