pipeline {
    agent any
	
	triggers {
		pollSCM('*H/2 * * * *')
	}
	
	parameters {
		string(name: 'MY_NAME', defaultValue: 'Gourish', description: 'What is my name ?')
	}
	
    stages {
		stage('Print maven version'){
			steps{
				echo "${MY_NAME}"
				bat 'mvn -v'
			}
		}
	}
}
