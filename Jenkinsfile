pipeline{
	agent any
	stages {
		stage("build") {
			steps {
				echo "mvn --version"
				sh "mvn clean install"
			}
		}
		stage("test"){
			steps {
				echo "Tesing..."
				sh "mvn test"
			
		}

	post {
		always {
			cleanWs()
		}
	}
}