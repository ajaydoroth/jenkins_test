
pipeline {
    agent any

    stages {
        stage('Git Checkout') {
            steps {
                echo 'Starting Git checkout stage'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'This is the build stage'
            }
        }

        stage('Test') {
            steps {
                echo 'This is the test stage'
            }
        }

        stage('Final Stage') {
            steps {
                echo 'Hi.... This is final stage...'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed. Check the console output.'
        }
    }
}

