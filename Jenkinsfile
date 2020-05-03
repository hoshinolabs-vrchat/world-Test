pipeline {
	agent none
	options {
		buildDiscarder(logRotator(numToKeepStr: '5'))
		disableResume()
		skipDefaultCheckout()
	}
	stages {
		stage('Pipeline') {
			when {
				branch 'master'
			}
			steps {
				build job: 'hoshinolabs-vrchat/world-Test-wrapper/master'
			}
		}
	}
}
