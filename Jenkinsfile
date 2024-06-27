pipeline {
    agent any // Run on any available agent

    stages {
        stage('Checkout Code') {
            steps {
                // Get code from your version control system (e.g., Git)
                git branch: 'main', // Replace with your branch name
                   credentialsId: 'your-credentials-id', // Replace with your credentials ID (if needed)
                   url: 'https://github.com/yahyagulshan/jenkinspipeline.git'
            }
        }
        stage('Build') {
            steps {
                // Perform build steps specific to your project (e.g., mvn clean install, npm install, etc.)
                sh 'mvn clean install' // Example using Maven
            }
        }
        stage('Test') {
            steps {
                // Run tests for your application (e.g., mvn test, npm test, etc.)
                sh 'mvn test' // Example using Maven
            }
        }
        // stage('Deploy (Optional)') {
        //     steps {
                // Deploy your application to a staging or production environment (optional)
                // You might need additional tools or configurations depending on your deployment method
            }
        }
    }
}
