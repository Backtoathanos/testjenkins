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
                echo "Pulling latest commits..."
                checkout scm
            }
        }

        stage('Verification After Pull') {
            steps {
                script {
                    if (isUnix()) {
                        sh 'ls -la'
                    } else {
                        bat 'dir'
                    }
                }
            }
        }

    }
}
