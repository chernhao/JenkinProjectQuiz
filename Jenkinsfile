pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
				sh 'composer install'
			}
		}
		stage('Test') {
			steps {
                // sh './vendor/bin/phpunit tests'
				sh' . /vendor/bin/phpunit——log-junit logs/unitreport.xmi -c tests/phpunit.xml tests'
            }
		}
	}
}
