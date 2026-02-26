pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Cratosaris/mon-projet-simple.git'
            }
        }
        stage('Test') {
            steps {
                sh 'python3 -m pytest --version'
            }
        }
        stage('Build') {
            steps {
                sh 'python3 main.py'
            }
        }
    }
}
