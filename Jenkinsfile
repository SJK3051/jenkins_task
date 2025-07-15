pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/SJK3051/jenkins_task.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
                // Example: sh 'mvn package' or 'npm install'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Example: sh 'mvn test' or 'npm test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying to staging...'
                // Example: sh './deploy.sh'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
