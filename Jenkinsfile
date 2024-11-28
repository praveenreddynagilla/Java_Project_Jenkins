pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the repository
                git 'https://github.com/praveenreddynagilla/Java_Project_Jenkins.git'
            }
        }

        stage('Build') {
            steps {
                // Build your project (example using Maven)
                sh 'mvn clean install'
            }
        }
    }

    post {
        success {
            echo "Build completed successfully"
        }
        failure {
            echo "Build failed"
        }
    }
}
