pipeline {
    agent any 
    tools {
        maven "Apache Maven 3.6.1"
    }
    stages {
        stage('--Clean--') { 
            steps {
                sh "mvn clean -f my-app"
            }
        }
        stage('--Test--') { 
            steps {
                sh "mvn test -f my-app"
            }
        }
        stage('--Deploy--') { 
            steps {
                sh "mvn package -f my-app"
            }
        }
    }
}