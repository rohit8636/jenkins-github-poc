pipeline {
    agent any

    triggers {
        pollSCM('H/2 * * * *')  // Poll every 5 minutes
    }

    stages {
        stage('Checkout') {
            steps {
                // Checkout code from GitHub main branch
                git branch: 'main', url: 'https://github.com/rohit8636/jenkins-github-poc.git'
            }
        }
        
        stage('Build') {
            steps {
                echo 'Building...'
                // Add your build commands here
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Add your test commands here
            }
        }
    }
}
