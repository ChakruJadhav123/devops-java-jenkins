pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning repository...'
            }
        }

        stage('Build') {
            steps {
                sh 'javac App.java'
            }
        }

        stage('Run') {
            steps {
                sh 'java App'
            }
        }
    }
}
