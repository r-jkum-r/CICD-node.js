pipeline {
    agent any

    tools {
        nodejs 'nodejs'
    }
    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/r-jkum-r/CICD-node.js.git'
            }
        }
        stage('Install') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }
    }
}
