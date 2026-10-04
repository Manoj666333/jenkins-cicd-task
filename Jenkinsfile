pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building Docker image...'
                sh 'docker build -t jenkins-cicd-app .'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing Docker container...'
                sh 'docker run --rm jenkins-cicd-app'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                sh 'docker rm -f jenkins-cicd-app-container 2>/dev/null || true'
                sh 'docker run -d --name jenkins-cicd-app-container jenkins-cicd-app'
            }
        }
    }
}
