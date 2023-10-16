pipeline {
    agent any

    stages {
        stage('SSH into Server') {
            steps {
                script {
                    def remote = [:]
                    remote.name = 'my-remote-server'
                    remote.host = 'ec2-3-96-163-214.ca-central-1.compute.amazonaws.com'
                    remote.user = 'ubuntu'
                    remote.privateKeyFile = credentials('MySSHPrivateKey')

                    sshCommand remote: remote, command: '''
                        echo "Hello from the remote server"
                        # Add more commands here
                    '''
                }
            }
        }
    }
}


