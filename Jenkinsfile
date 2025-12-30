pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    sh ""
                    echo "Building"
                    ""
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    sh ""
                    echo "Building"
                    }    "" 
            }
        }
        stage('Deploy') {
            steps {
            script {
                    sh ""
                    echo "Building"
                    ""
            }
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