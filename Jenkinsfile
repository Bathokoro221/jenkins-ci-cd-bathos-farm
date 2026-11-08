pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out code...'
                checkout scm
            }
        }
        stage('Build') {
            steps {
                echo 'Building Bathos Farm App...'
                sh 'ls -la'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'test -f index.html && echo "index.html found"'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying Bathos Farm App...'
            }
        }
    }
}
