pipeline {

    agent { label 'linux' }

    stages {

        stage('Clone Code') {
            steps {
                echo "Cloning repository..."
                git 'https://github.com/Cratosaris/jenkins-demo-app.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building application..."
            }
        }

        stage('Test') {
            steps {
                sh 'ls -l'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                sudo cp index.html /var/www/html/index.html
                '''
            }
        }

    }
}
