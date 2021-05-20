pipeline {
	agent any
		stages {
			stage('First') {
				steps {
					sh '''
						echo "Step One"
					'''
				}
				steps {
					script {
						env.EXECUTE="True"
					}
				}
			}


			stage('Second') {
				when {
					expression { EXECUTE == "True"}
				}
				steps {
					sh '''
						echo "Updating Second Stage"
					'''
				}
				steps {
					script {
						echo "${EXECUTE}"
					}
				}
				
			} 

			stage('Third') {
				steps {
					sh '''
						echo "Step Three"
					'''
				}
			}
		}
	}
}
