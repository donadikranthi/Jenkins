pipeline {
       agent {
            node {
               label 'AGENT-1' // Replace with your actual node label
       }
 }

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