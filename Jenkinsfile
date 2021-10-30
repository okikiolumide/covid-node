pipeline{
	agent none
		stages{
			stage('SCM' ){
				steps{
					echo "Cloning Git Repo"
					
				}
			}
			stage('Run Security Test') {
						parallel {
							stage('Check for Security Vulnerabilities') {
								
								steps {
									echo "run-tests.bat"
								}
							}
							
							stage('Another Security Test') {
								
								steps {
									echo "run-tests.sh"
								}
								
							}
						}
			}

			stage('Build'){
				steps{
					echo "Building Docker File" 

				}
			}

			stage('Run Tests') {
						parallel {
							stage('Test On Windows') {
								
								steps {
									echo "run-tests.bat"
								}
							}
							
							stage('Test On Linux') {
								
								steps {
									echo "run-tests.sh"
								}
								
							}
						}
			}

		}
	}

