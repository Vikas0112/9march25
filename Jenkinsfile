
pipeline {
    agent any

    
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/your-repo/example.git'
            }
        }

        stage('Build') {
            steps {
                sh './build.sh'
            }
        }

    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}
