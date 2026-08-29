pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo "Building the code using Maven to compile and package the application."
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo "Running unit tests with JUnit to verify individual components work as expected."
                echo "Running integration tests with Postman/Newman to verify components work together correctly."
            }
        }

        stage('Code Analysis') {
            steps {
                echo "Analysing code quality and maintainability using SonarQube."
            }
        }

        stage('Security Scan') {
            steps {
                echo "Scanning the code for vulnerabilities using OWASP ZAP."
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo "Deploying the application to a staging server (AWS EC2 instance)."
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo "Running integration tests on the staging environment using Postman/Newman to confirm the app behaves correctly in a production-like setting."
            }
        }

        stage('Deploy to Production') {
            steps {
                echo "Deploying the application to a production server (AWS EC2 instance)."
            }
        }
    }
}
