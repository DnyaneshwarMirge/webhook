pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                // Clone code from GitHub repository
                git url: 'https://github.com/username/repo.git', branch: 'main'
            }
        }

        stage('Build') {
            steps {
                // Simple print message to indicate the build stage
                echo 'Building project...'
            }
        }

        stage('Test') {
            steps {
                // Here you can run test commands (e.g., npm test, mvn test)
                echo 'Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                // You can add deployment logic here
                echo 'Deploying the application...'
            }
        }
    }

    post {
        always {
            // This block runs after the pipeline, regardless of status
            echo 'Build finished.'
        }
    }
}
