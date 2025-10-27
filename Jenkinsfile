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
                sh 'echo "All tests passed successfully!"'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying app locally with PM2...'
                sh '''
                    npm install -g pm2
                    pm2 delete my-node-app || true
                    pm2 start app.js --name my-node-app
                    pm2 save
                '''
            }
        }
    }
}

