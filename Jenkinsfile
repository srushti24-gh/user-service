pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Building from feature branch: ${env.BRANCH_NAME}"
                bat 'python app.java'
            }
        }
        stage('Test') {
            steps {
                echo "Running feature branch tests..."
                bat 'echo Simulating feature testing...'
            }
        }
    }
}
