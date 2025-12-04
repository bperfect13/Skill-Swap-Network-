pipeline {
    agent {
        docker {
            image 'python:3.10-slim'
        }
    }

    stages {
        stage('Checkout SCM') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Running build in Python container...'
                sh 'python --version'
                sh 'python app.py'
            }
        }
    }
}
