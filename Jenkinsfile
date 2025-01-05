pipeline {
    agent any
    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/username/repo.git'
            }
        }
        stage('Build') {
            steps {
                sh 'python test.py'  // Use 'bat' instead of 'sh' for Windows
            }
        }
        stage('Test') {
            steps {
                sh 'python -m unittest discover'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
            }
        }
    }
}
