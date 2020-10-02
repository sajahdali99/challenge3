pipeline {
	agent any
	stages {
		stage('Build Images Push Images'){
			steps {
				sh "./buildscript.sh"
			}
		}
		stage('Push Images'){
			steps {
				sh "./pushscript.sh"
			}
		}
		stage('Test Containers'){
			steps {
				sh "./testscript.sh"
			}
		}
	}
}
