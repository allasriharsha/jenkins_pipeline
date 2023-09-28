

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                Secret_key=$SSH_KEY
                sh 'echo Building...'
                sh 'echo "Using API key: $Secret_key"'
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
