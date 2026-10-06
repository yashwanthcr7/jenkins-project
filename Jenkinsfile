pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                sh '''
                    echo "Building application..."
                    chmod +x app.sh
                '''
            }
        }

        stage('Test') {
            steps {
                sh '''
                    ./app.sh
                '''
            }
        }

        stage('yash') {
            steps {
                sh '''
                cat sample
                '''
            }
        }

        
        stage('Deploy') {
            steps {
                echo "Deploying application..."
            }
        }
    }
}
