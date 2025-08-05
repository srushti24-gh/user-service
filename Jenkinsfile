pipeline {
    agent any
    environment {
        ENABLE_FEATURE_X = 'true'  // or pull from `.env` or repo file
    }
    stages {
        stage('Build') {
            steps {
                echo "Compiling Java..."
                bat 'javac app.java'
            }
        }
        stage('Run') {
            steps {
                echo "Running App..."
                bat 'java app'
            }
        }
        stage('Feature Toggle') {
            when {
                expression { return env.ENABLE_FEATURE_X == 'true' }
            }
            steps {
                echo '✅ Feature X is ENABLED – Running feature-specific code...'
            }
        }
    }
}
