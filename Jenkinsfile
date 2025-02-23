pipeline {
    agent any
    tools {
        maven 'Maven'  // Name of Maven tool configured in Jenkins
    }
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
    }
}