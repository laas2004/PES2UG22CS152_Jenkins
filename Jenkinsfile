pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'g++ -o YOUR_SRN-1 YOUR_SRN.cpp' // Replace YOUR_SRN with your actual SRN
            }
        }

        stage('Test') {
            steps {
                echo 'Testing the application...'
                sh './YOUR_SRN-1' // Execute the compiled C++ program
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
