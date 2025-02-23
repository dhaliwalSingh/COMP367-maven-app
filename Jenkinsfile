pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/dhaliwalSingh/COMP367-maven-app.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Deploy') {
            steps {
                echo "Deployment Completed"
            }
        }
    }
}