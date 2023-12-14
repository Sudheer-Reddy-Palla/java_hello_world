pipeline {
    agent any // Allows Jenkins to run the pipeline on any available agent

    stages {
        stage('Checkout') {
            steps {
                checkout scm // Fetches the code from your Git repository
            }
        }

        stage('Build') {
            steps {
                // Compile your Java code
                sh 'javac HelloWorld.java'
            }
        }

        stage('Run') {
            steps {
                // Run your Java program
                sh 'java HelloWorld'
            }
        }
    }
}
