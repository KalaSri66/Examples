
pipeline {
	agent any
	stages {
			stage ('Initialize') {
				steps {
					sh ''' 
						echo "PATH = ${PATH}"
						echo "M2 HOME = ${M2_HOME}"
						'''
				}
			}
			stage ('Build') {
				steps {
					echo 'Hello World!'
				}
			}
	}
}