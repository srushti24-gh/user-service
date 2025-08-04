pipeline {
    agent any
    environment {
        ENV = 'staging'  // You can change to 'production' as needed
    }
    stages {
        stage('Build') {
            steps {
                echo "Building ${env.ENV} environment..."
                // Add actual build commands here
            }
        }
        stage('Test') {
            steps {
                echo "Running tests..."
                // Add test commands (e.g., npm test, mvn test, etc.)
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying to ${env.ENV}..."
                // Add deploy commands here
            }
        }
    }
}
