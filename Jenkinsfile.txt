pipeline {
	agent any 
	stages {
		stage('Build') {
			steps {
					sh 'sleep 3; echo "This is build stage"'
				}
			}
		stage('Test') {
			steps {
				sh '''
					sleep 3
					echo "This is Test stage"
					'''
				}
			}
		stage('Deploy') {
			steps {
				sh '''
					sleep 3
					echo "This is Deploy stage"
					'''
				}
			}
		}

}