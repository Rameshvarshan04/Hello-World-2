pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Pulling the source code from GitHub
                git branch: 'master', url: 'https://github.com/Rameshvarshan04/Hello-World-2.git'
            }
        }

        stage('Build') {
            steps {
                script {
                    // Dummy build step for a simple Hello World app
                    echo 'Building the Hello World application...'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    // Dummy test step for Hello World
                    echo 'Running tests for the Hello World application...'
                }
            }
        }

        stage('Run Application') {
            steps {
                script {
                    // Dummy run step
                    echo 'Hello World application is running!'
                }
            }
        }
    }

    post {
        always {
            // Clean up workspace after build
            cleanWs()
        }
    }
}
