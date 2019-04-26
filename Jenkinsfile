pipeline{
	enviroment{
		registry = "elidockertest/d4a3"
		registryCredential = "dockerhub"
	}
	agent any
	stages{
		stage('Starting'){
			steps{
				sh 'echo starting....'
			steps{
				sudo docker ps
			}
		stage('Build Image'){
			steps{
			script{
				dockerImage=docker.build registry + ":$BUILD_NUMBER"
			}
			}
		stage('Push Image DockerHub'){
			steps{
				script{
					docker.withRegisitry('',registryCredential)
				}
			}
		}
		}
			}
		}
	}
