@Library('shared-lib') _

pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/<your-username>/jenkins-ci-demo.git'
            }
        }

        stage('Docker Build using Shared Library') {
            steps {
                dockerBuild('demo-app')
            }
        }
    }
}
