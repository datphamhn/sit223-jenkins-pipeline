// test trigger 
//test trigger v2
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Task: Compile and package the source code into a deployable artifact.'
                echo 'Tool: Maven'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Task: Run unit tests to verify individual components work as expected, and integration tests to check that components interact correctly together.'
                echo 'Tool: JUnit for unit testing, Postman/Newman for integration testing'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Task: Analyse the codebase for code smells, complexity, and adherence to coding standards.'
                echo 'Tool: SonarQube'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Task: Scan the code and its dependencies for known security vulnerabilities.'
                echo 'Tool: OWASP Dependency-Check'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Task: Deploy the built application to a staging server for pre-production testing.'
                echo 'Tool: AWS EC2 instance with Ansible for deployment automation'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Task: Run integration tests against the staging environment to confirm the application behaves correctly in a production-like setting.'
                echo 'Tool: Selenium'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Task: Deploy the verified application build to the production server.'
                echo 'Tool: AWS EC2 instance with Ansible for deployment automation'
            }
        }
    }
}
