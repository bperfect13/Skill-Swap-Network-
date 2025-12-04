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
                sh '''
                  apt-get update
                  apt-get install -y python3
                  python3 app.py
                '''
            }
        }
    }
}
