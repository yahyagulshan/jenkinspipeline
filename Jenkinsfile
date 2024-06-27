pipeline {
  agent any

  stages {
    stage('Checkout Code') {
      steps {
        git branch: 'main',
           credentialsId: 'github',
           url: 'https://github.com/yahyagulshan/jenkinspipeline/edit/main/Jenkinsfile.git'
      }
    }
    stage('Build') {
      steps {
        sh 'make clean && make' // Replace 'make' with your build command
      }
    }
  }
}
