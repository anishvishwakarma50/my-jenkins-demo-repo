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
                echo 'Simulating build...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'python test.py'
            }
        }
    }

    post {
        always {
            echo 'Pipeline completed.'
        }
    }
}
