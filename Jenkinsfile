pipeline {

    agent any
    
    stages {
         stage('Checkout') {
            steps {
                git 'https://github.com/ProCodingTech/SCDlab11.git'
            }
        }
        stage('Dependency Installation') {
            steps {
                sh 'npm install'
            }
        }
        stage('Build Docker Image') {
        steps {
                sh 'echo docker build -t your-image-name .'
            }
        }
        stage('Push Docker Image') {
        steps {
                sh 'echo docker push your-registry/your-image-name'
            }
        }
    }
}
