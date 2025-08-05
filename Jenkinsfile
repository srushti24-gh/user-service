pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Building from develop branch..."
                bat 'javac app.java'
            }
        }
        stage('Test') {
            steps {
                echo "Running tests for develop..."
                bat 'echo Simulating tests...'
            }
        }
    }
}
