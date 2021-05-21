pipeline {
	agent any
	environment {
	        FOO = "bar"
	}
		stages {
			stage('First') {
				
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


			stage('Second') {
				steps {
					sh '''
						echo "Step -Two"
					'''
				}
			} 

			stage('Third'){
				steps {
					sh '''
						echo "Step -Three"
					'''
				}
			}
		}
}
