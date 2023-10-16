pipeline {
    agent any
environment {
        //SECRET_KEY_FILE = '/var/lib/jenkins/salla.pem'
        SSH_HOST = 'ec2-3-96-163-214.ca-central-1.compute.amazonaws.com'
    }
    stages {
        stage('Build') {
            steps {
                
                sh 'echo Building...'
                sh 'echo "Using API key: $SSH_KEY"'
                script {
                    
                    def commands = [
                        'echo "Hello, world!"',
                        'ls -l /path/to/some/directory'
                    ]
                withCredentials([sshUserPrivateKey(credentialsId: 'MySSHPrivateKey', keyFileVariable: 'SSH_KEY')]) {
                    sh """
                    # You can use SSH_KEY as the private key file in your SSH command
                   
                    ssh -o StrictHostKeyChecking=no -i \$SSH_KEY ubuntu@$SSH_HOST <<EOF
                    whoami
                    ls -a
                    EOF
                    """
                   
                 
                }


                    
                }
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
