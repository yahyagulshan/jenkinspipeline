pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/yahyagulshan/jenkinspipeline.git'
            }
        }

        stage('Build') {
            steps {
                // Example build step - replace with your actual build commands
                sh 'echo "Building the project..."'
            }
        }

        stage('Test') {
            steps {
                // Example test step - replace with your actual test commands
                sh 'echo "Running tests..."'
            }
        }

        stage('Deploy') {
            steps {
                // Example deploy step - replace with your actual deployment commands
                sh 'echo "Deploying the project..."'
            }
        }
    }

    post {
        success {
            echo 'Pipeline succeeded!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}

