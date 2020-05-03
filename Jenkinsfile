pipeline {
	agent none
	options {
		buildDiscarder(logRotator(numToKeepStr: '5'))
		disableResume()
		skipDefaultCheckout()
	}
	stages {
		stage('Pipeline') {
			steps {
				script {
					def job = build job: 'world-Test-wrapper/master'
				}
			}
		}
	}
}
