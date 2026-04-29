pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Fetching code...'
                git 'https://github.com/your-username/your-repo.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Compiling...'
                bat 'javac ArmstrongNumbers.java'
            }
        }

        stage('Test') {
            steps {
                echo 'Executing program...'
                bat 'java ArmstrongNumbers'
            }
        }

        stage('Archive') {
            steps {
                archiveArtifacts artifacts: '*.class'
            }
        }
    }
}
