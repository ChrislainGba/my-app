pipeline {
    agent any 
    tools {
        maven "Apache Maven 3.6.1"
    }
    stages {
        stage('--Clean--') { 
            steps {
                sh "mvn clean"
            }
        }
        stage('--Test--') { 
            steps {
                sh "mvn test"
            }
        }
        stage('--Deploy--') { 
            steps {
                sh "mvn package"
            }
        }
    }
}