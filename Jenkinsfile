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
				steps {
					sh '''
						echo "Step -Two"
					'''
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
