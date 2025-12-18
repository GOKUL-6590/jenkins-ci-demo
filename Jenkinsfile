@Library('jenkins-shared-lib') _

pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/GOKUL-6590/jenkins-ci-demo.git'
            }
        }

        stage('Docker Build using Shared Library') {
            steps {
                dockerBuild('demo-app')
            }
        }
    }
}
