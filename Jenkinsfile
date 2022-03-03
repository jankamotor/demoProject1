pipeline {
    agent any

    stages {
        stage('Sonar-test') {
	steps {
            withSonarQubeEnv('My SonarQube Server') {
  
            println "${env.SONAR_HOST_URL}" 
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
