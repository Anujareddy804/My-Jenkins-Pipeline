pipeline {
    agent any   // Runs on any available Jenkins agent

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/Anujareddy804/My-Jenkins-Pipeline.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'  // Replace with actual build commands
                sh 'chmod +x Anuja.sh && ./Anuja.sh'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'  // Replace with actual test commands
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'  // Replace with actual deployment commands
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
