pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Building from master branch..."
                bat 'python app.java'
            }
        }
        stage('Test') {
            steps {
                echo "Testing on master branch..."
                bat 'echo Simulating final tests...'
            }
        }
        stage('Deploy') {
            when {
                branch 'master'
            }
            steps {
                echo "🚀 Deploying to production from master branch..."
                bat 'echo Deploy script runs here'
            }
        }
    }
}
