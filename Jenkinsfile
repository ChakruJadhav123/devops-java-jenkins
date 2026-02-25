pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                echo 'Cloning from GitHub...'
                git 'https://github.com/ChakruJadhav123/devops-java-jenkins.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                echo 'Building Docker image...'
                sh 'docker build -t java-devops-app .'
            }
        }

        stage('Run Docker Container') {
            steps {
                echo 'Running Docker container...'
                sh 'docker run --rm java-devops-app'
            }
        }

    }
}
