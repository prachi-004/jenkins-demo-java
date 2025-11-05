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
                bat 'mkdir out'
                bat 'javac -d out src_java\\HelloWorld.java'
                bat 'java -cp out HelloWorld'
            }
        }
    }
}
