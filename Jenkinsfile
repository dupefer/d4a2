pipeline{
	agent any
	stages{
		stage ('Initial Setup'){
			steps{
				sh 'echo Starting...'
			}
		}
		stage ('Checking Docker'){
			steps{
				sh 'sudo docker ps'
			}
		}
		stage ('Build Docker'){
			steps{ sh 'echo Fase Build'
				sh 'sudo docker build --tag=php54  .'
			}
		}
		stage ('Deploy Cointainer'){
			steps{ sh 'echo Fase Deploy'
				sh 'sudo docker-compose down'
				sh 'sudo docker-compose up -d'		
			}
		}
	}
}
