pipeline{
	agent{
		dockerfile true
		}
		stages{
			stage('SCM' )
				steps{
					echo "Cloning Git Repo"
					git credentialsId: '62fe0952-3d55-4055-a11b-17559fcae927', url: 'https://github.com/okikiolumide/covid-node.git '
				}

			stage('Build')
				steps{
					echo "Building Docker File" 

				}

		}
}
