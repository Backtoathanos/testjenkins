pipeline {
    agent any

    stages {

        stage('Checking for New Commits') {
            steps {
                echo "Checking for new commits..."
            }
        }

        stage('Pulling Latest Code') {
            steps {
                script {
                    echo "Pulling latest commits..."
                }
                checkout scm
            }
        }

        stage('Verification After Pull') {
            steps {
                script {
                    echo "Code pulled successfully!"
                    sh 'ls -la'
                }
            }
        }
    }
}
