pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/tusharbiswas9038/Jenkins-CI-Pipeline-PythonApp'
            }
        }
        stage('Install Dependencies') {
            steps {
                sh 'pip install -r requirements.txt'
            }
        }
        stage('Test') {
            steps {
                sh 'pip install pytest && pytest test_app.py'
            }
        }
    }
}
