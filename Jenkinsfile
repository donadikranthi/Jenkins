pipeline {
    agent any // This means that the pipeline can run on any available agent
    stages {  
        stage('Build') {
            steps {
                echo 'Building...'
                // Add your build commands here, e.g., sh 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Add your test commands here, e.g., sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add your deploy commands here, e.g., sh 'mvn deploy'
            }
        }
    }
}