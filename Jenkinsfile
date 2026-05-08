pipeline {
    agent any

    stages {

        stage('Compile') {
            steps {
                echo 'Compiling Java code...'
                bat 'mvn clean compile'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                bat 'mvn test'
            }
        }

        stage('Package') {
            steps {
                echo 'Packaging app...'
                bat 'mvn package'
            }
        }
    }
}