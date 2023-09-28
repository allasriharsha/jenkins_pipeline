

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                SECRET_KEY=credentials("yey")
                sh 'echo Building...'
                sh 'echo "Using API key: $SECRET_KEY"'
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
