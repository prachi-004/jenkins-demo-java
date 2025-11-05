pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/<your-username>/jenkins-demo-java.git'
            }
        }

        stage('Build') {
            steps {
                sh 'bash build.sh'
            }
        }
    }
}
