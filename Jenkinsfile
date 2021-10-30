pipeline{
	agent none
		stages{
			stage('SCM' ){
				steps{
					echo "Cloning Git Repo"
					
				}
			stage('Security Checks){
				       steps{
					echo "Running Security Checks"
				       }
				}
				
		}

			stage('Build'){
				steps{
					echo "Building Docker File" 

				}
			}

		}
}
