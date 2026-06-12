pipeline {
       agent {
            node {
               label 'AGENT-1' // Replace with your actual node label
       }
 }

    stages {  
        stage('Build') {
            steps {
                 script {
                    sh """
                    echo "Building..."
                    echo $COURSE
                    """
                    
                // Add your build commands here, e.g., sh 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                 script {
                    sh """
                    echo "Testing..."
                    """
                // Add your test commands here, e.g., sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                 script {
                    sh """
                    echo "Deploying..."
                    """
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