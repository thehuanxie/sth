pipeline {
	agent {
		docker {
			image 'maven:3.9.0-eclipse-temurin-17'
			args '-v /root/.m2:/root/.m2'
		}
	}
	stages {
		stage('build') {
			steps {
				sh 'mvn -B clean package'
			}
		}
	}
}
