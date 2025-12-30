pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                steps {
                    sh """
                    echo "Building"
                    """
                }
            }
        }
        stage('Test') {
            steps {
                echo "Testing"
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying"
            }
        }
    }
        post {
            always {
                echo "I will always say Hello World!"
                cleanWs()
            }
            success {
                echo "I succeeded!"
            }
            failure {
                echo "I failed!"
            }
        }
        }