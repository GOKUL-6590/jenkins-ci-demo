pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'echo Build completed'
            }
        }

        stage('Test') {
            steps {
                sh 'echo Tests passed'
            }
        }

        stage('Docker Build') {
            steps {
                sh 'docker build -t demo-app .'
            }
        }

        stage('Docker Push') {
            steps {
                sh 'echo Docker push step'
            }
        }
    }
}
