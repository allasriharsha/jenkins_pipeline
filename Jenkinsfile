pipeline {
    agent any

    stages {
        stage('SSH into EC2 and Run Commands') {
            steps {
                script {
                    def remote = [:]
                    remote.name = 'my-ec2-instance'
                    remote.host = 'ec2-3-96-163-214.ca-central-1.compute.amazonaws.com'
                    remote.user = 'ubuntu'  // Use the appropriate SSH username
                    remote.identityFile = credentials('MySSHPrivateKey')

                    // SSH into the EC2 instance and execute commands
                    remote.command = """
                        ls -l
                        whoami
                        # Add more commands here
                    """
                    sshPut remote: remote
                }
            }
        }
    }
}
