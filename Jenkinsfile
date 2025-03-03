pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/<your-username>/<repo-name>.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the application...'
            }
        }
        stage('Test') {
            steps {
                sh 'python -m unittest discover'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
}