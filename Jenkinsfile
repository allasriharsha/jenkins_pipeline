

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                SECRET_KEY_FILE="/var/lib/jenkins/salla.pem"
                sh 'echo Building...'
                sh 'echo "Using API key: $SSH_KEY"'
                ssh -i "$SECRET_KEY_FILE" ubuntu@ec2-3-96-163-214.ca-central-1.compute.amazonaws.com
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
