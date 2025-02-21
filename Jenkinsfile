pipeline {
    agent any
    stages {
        stage('NPM Install') {
            steps {
                bat 'npm install'
            }
        }
        stage('Run npm audit') {
            steps {
                bat 'npm audit'
            }
        }
        stage('Run Integration tests') {
            steps {
                bat 'npm run test'
            }
        }
        stage('Deploy to STAGING') {
            steps {
                echo 'Deploying to staging'
            }
        }
        stage('Deploy to PRODUCTION') {
            steps {
                echo 'Deploying to production'
            }
        }
    }
}
