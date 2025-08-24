pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/mohammedsaifsgp/jen2.git'
            }
        }
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t myapp:latest .'
            }
        }
    }
}
