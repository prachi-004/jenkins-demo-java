pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/prachi-004/jenkins-demo-java.git'
            }
        }

        stage('Build') {
            steps {
                // Create output folder if not exists
                bat 'if not exist out mkdir out'
                
                // Compile Java from src_java
                bat 'javac -d out src_java\\HelloWorld.java'
                
                // Run the program
                bat 'java -cp out HelloWorld'
            }
        }
    }
}
