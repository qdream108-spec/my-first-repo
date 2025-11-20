# my-first-repo
pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                echo "Pulling code from repository..."
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo "Building the project..."
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying application..."
            }
        }
    }
}

