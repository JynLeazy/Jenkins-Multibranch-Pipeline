pipeline {
	agent any
		stages {
			stage('First') {
				steps {
					sh '''#!/bin/bash
						echo "Step -One"
					'''
				}
			}


			stage('Second') {
				steps {
					sh '''#!/bin/bash
						echo "Step -Two"
					'''
				}
			} 

			stage('Third'){
				steps {
					sh '''#!/bin/bash
						echo "Step -Three"
					'''
				}
			}
		}
}
