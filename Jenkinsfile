pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                bat 'javac ArmstrongNumbers.java'
            }
        }

        stage('Test') {
            steps {
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
