pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'g++ -o PES2UG22CS152-1 PES2UG22CS152.cpp' // Replace YOUR_SRN with your actual SRN
            }
        }

        stage('Test') {
            steps {
                echo 'Testing the application...'
                sh './PES2UG22CS152-1' // Execute the compiled C++ program
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Add deployment steps here (e.g., copying files to a server)
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed!'
        }
    }
}
