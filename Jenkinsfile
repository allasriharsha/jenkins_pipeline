

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
            
                sh 'echo Building...'
                sh 'echo "Using API key: $SSH_KEY"'
            }
        }
        stage('Test') {
            steps {
                sh 'echo Testing...'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo Deploying...'
            }
        }
    }
}
