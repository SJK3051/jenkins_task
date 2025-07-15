pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Replace with your repo URL
                git 'https://github.com/SJK3051/jenkins_task.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
                // Example build command
                // sh 'make build' or 'npm install'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Example test command
                // sh 'npm test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                // Example deploy step
                // sh './deploy.sh'
            }
        }
    }
}

