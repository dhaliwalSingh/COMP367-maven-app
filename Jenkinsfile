pipeline {
    agent any
    environment {
        PATH = "/opt/homebrew/bin:$PATH"
        M2_HOME = "/opt/homebrew/Cellar/maven/3.x.x/libexec"
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
        stage('Deploy') {
            steps {
                echo "Deployment Completed"
            }
        }
    }
}