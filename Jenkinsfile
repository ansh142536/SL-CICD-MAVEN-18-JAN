pipeline {
    agent any
    
    tools {
        maven 'local_maven'  // Name of the Maven installation in Jenkins
        jdk 'JDK'      // Name of the JDK installation in Jenkins
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/your-repo.git'  // Replace with your repository URL
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                // Add deployment steps if needed
            }
        }
    }
}

