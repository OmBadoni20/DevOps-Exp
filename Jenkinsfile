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

        stage('Test') {
            steps {
                bat 'if exist Main.class (echo Test Passed: Main.class created successfully) else (echo Test Failed & exit /b 1)'
            }
        }

        stage('Run') {
            steps {
                bat 'java Main'
            }
        }
    }
}
