pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building Node.js app...'
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'npm test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment simulation complete!'
            }
        }
    }
}

