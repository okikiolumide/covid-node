pipeline{
	agent none
		stages{
			stage('SCM' ){
				steps{
					echo "Cloning Git Repo"
					
				}
				steps{
					echo "Running Security Checks"
					
				}
				steps{
					echo "Unit Testing"
					
				}
		}

			stage('Build'){
				steps{
					echo "Building Docker File" 

				}
			}

		}
}
