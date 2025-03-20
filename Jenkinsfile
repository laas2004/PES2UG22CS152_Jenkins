pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'g++ -o PES2UG22CS152-1 PES2UG22CS152.cpp' // Compile the .cpp file
            }
        }

        stage('Test') {
            steps {
                echo 'Testing the application...'
                sh './PES2UG22CS152-1' // Execute the compiled program
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
