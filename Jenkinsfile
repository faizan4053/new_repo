pipeline{
	agent any
	stages {
		stage("Build") {
			steps {
				sh "mvn --version"
				sh "mvn clean install"
			}
		}
		stage("Test"){
			steps {
				sh "Tesing..."
				sh "mvn test"
			
		}

	post {
		always {
			cleanWs()
		}
	}
}