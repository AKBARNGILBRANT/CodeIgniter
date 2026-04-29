pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'develop', url: 'https://github.com/AKBARNGILBRANT/CodeIgniter.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building CodeIgniter...'
                sh 'ls -la'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'echo "Test berhasil"'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                sh 'echo "Deploy simulasi selesai"'
            }
        }
    }

    post {
        success {
            echo 'Pipeline berhasil dijalankan dengan sukses!'
        }
        failure {
            echo 'Terjadi kegagalan pada pipeline!'
        }
    }
}
