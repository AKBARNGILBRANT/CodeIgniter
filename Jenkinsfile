pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/AKBARNGILBRANT/CodeIgniter.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building CodeIgniter...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }

    post {
        success {
            echo 'Pipeline berhasil!'
        }
        failure {
            echo 'Pipeline gagal!'
        }
    }
}
