pipeline {

    agent any
    
    stages {
         stage('Checkout') {
            steps {
                sh 'echo CheckOut Passed'
            }
        }
        stage('Dependency Installation') {
            steps {
                sh 'npm install'
            }
        }
        stage('Start') {
            steps {
                sh 'npm start'
            }
        }
        stage('Build Docker Image') {
        steps {
                sh 'echo docker build -t SCDlab11'
            }
        }
        stage('Docker Comopse Up') {
            steps {
                    sh "docker compose up"
            }
        }
    }
}
