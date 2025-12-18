pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/GOKUL-6590/jenkins-ci-demo.git'
            }
        }

        stage('Build') {
            steps {
                sh 'echo Build stage'
            }
        }

        stage('Test') {
            steps {
                sh 'echo Test stage'
            }
        }

        stage('Docker Build') {
            steps {
                sh 'docker build -t demo-app .'
            }
        }

        stage('Docker Push') {
            steps {
                sh 'echo Docker push skipped (demo)'
            }
        }
    }
}
