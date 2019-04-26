pipeline{
	enviroment{
		registry = "elidockertest/d4a3"
		registryCredential = "HakunaMatata01"
	}
	agent any
	stages{
		stage('Starting'){
			steps('starting'){
				sh 'echo starting....'
		stage('Build Image'){
			steps{
			script{
				dockerImage=docker.build registry + ":$BUILD_NUMBER"
			}
			}
		}
			}
		}
	}
}
