pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Compile') {
            steps {
                bat 'javac Main.java'
            }
        }

        stage('Run') {
            steps {
                bat 'java Main'
            }
        }
    }
}
