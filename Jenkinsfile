pipeline {
	agent any
	environment {
	        FOO = "bar"
	}
		stages {
			stage('first') {
				
						
				steps {
					sh '''
						echo "Step -One"
					'''
					script {
						env.JORGE = "True"
					}
				}
			}


			stage('second') {
				when {
					expression { EXECUTE == "True"}
				}
				steps {
					sh '''
						echo "Step -Two"
						echo "Updating Second Stage"
					'''
					script {
						echo "${EXECUTE}"
					}
				}
			} 

			stage('third'){
				steps {
					sh '''
						echo "Step -Three"
					'''
				}
			}
		}
}
