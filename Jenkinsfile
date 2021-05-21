pipeline {
	agent any
	environment {
	        FOO = "bar"
	}
		stages {
			stage('first') {
				
				steps {
					script {
						env.JORGE = "True"
					}
				}
			
				steps {
					sh '''
						echo "Step -One"
					'''
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
