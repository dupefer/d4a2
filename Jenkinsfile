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
			}
		}
		stage {'Deploy Cointainer'){
			steps{ sh 'echo Fase Deploy'		
			}
		}
	}
}
