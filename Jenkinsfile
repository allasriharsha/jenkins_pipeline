

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                SECRET_KEY_FILE="/var/lib/jenkins/salla.pem"
                SSH_HOST="ec2-3-96-163-214.ca-central-1.compute.amazonaws.com"
                sh 'echo Building...'
                sh 'echo "Using API key: $SSH_KEY"'
                def sshCommand = """
                        ssh -i '$SECRET_KEY_FILE' ubuntu@$SSH_HOST
                    """
                // Execute the SSH command
                    sh(sshCommand)
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
