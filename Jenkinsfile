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
                bat 'type notes.txt'
            }
        }
    }

    post {
        always {
            echo 'Pipeline completed.'
        }
    }
}
