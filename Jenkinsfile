pipeline {
    agent any

    stages {
        stage('Sonar-test') {
	steps {
            withSonarQubeEnv('sonar') {
  
           
	    sh 'mvn clean package sonar:sonar'	 
}}
                
            
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
