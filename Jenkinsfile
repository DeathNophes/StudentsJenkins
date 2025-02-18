pipeline {
    agent any
    stages {
        stage('NPM Install') {
            steps {
                sh 'npm install'
            }
        }
        stage('Run npm audit') {
            steps {
                sh 'npm audit'
            }
        }
        stage('Run Integration tests') {
            steps {
                sh 'npm run test'
            }
        }
    }
}
