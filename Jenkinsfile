@Library('jenkins-shared-lib') _

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

        stage('Docker Build using Shared Library') {
            steps {
                dockerBuild('demo-app:latest')
            }
        }
    }
}
