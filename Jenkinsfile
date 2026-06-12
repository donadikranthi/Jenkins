pipeline {
       agent {
            node {
               label 'AGENT-1' // Replace with your actual node label
       }
 }
  environment {
        COURSE = "Jenkins"
    }
    // options {
    //     timeout(time: 10, unit: 'MINUTES') 
    //     disableConcurrentBuilds()
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
    post {
        always {
            echo 'I will always says hello.'
            cleanWs() // Clean workspace after the pipeline execution
        }
        success {
            echo 'Pipeline succeeded.'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }

}