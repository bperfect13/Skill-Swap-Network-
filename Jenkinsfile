pipeline {
    agent any

    stages {
        stage('Checkout SCM') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Running build...'
                sh 'echo "Hello from Jenkins build via Docker + GitHub!"'
            }
        }
    }
}
