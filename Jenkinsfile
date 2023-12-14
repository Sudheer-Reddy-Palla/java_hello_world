pipeline {
    agent {
        docker {
            // Specify the Docker image to be used as an agent
            image 'your_docker_image:tag' // Replace 'your_docker_image:tag' with your actual Docker image
            args '-v /var/run/docker.sock:/var/run/docker.sock' // Mount Docker socket for Docker commands in Jenkins
        }
    }
    stages {
        stage('Build') {
            steps {
                // Define your build steps here
                sh 'javac HelloWorld.java' // Example: Compile Java code
            }
        }
        stage('Run') {
            steps {
                // Run Java program
                sh 'java HelloWorld'
            }
        }
    }
}
