pipeline {
	agent none
	stages {
		stage('Build') {
			agent {
				docker {
					image 'python:2-alpine'
					}
			}
			steps {
				sh 'pwd'
				sh 'ls -la'
				sh 'python -m py_compile sources/add2vals.py sources/cals.py'
			}
		}
	}
}

