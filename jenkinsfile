pipeline {
    agent any

    triggers {
        // This tells Jenkins to look for GitHub webhook triggers
        githubPush()
    }

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out code from GitHub...'
                checkout scm
            }
        }
        stage('Build') {
            steps {
                echo 'Building the application...'
                // Add your build commands here (e.g., sh 'python -m compileall .')
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
    }
}
