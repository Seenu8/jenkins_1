pipeline {
    agent any

    tools {
        maven 'Maven_3'  // Name from Global Tool Configuration
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building the Code..........'
                bat 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                echo 'Running the tests...'
                bat 'mvn test'
            }
        }

        stage('Compile') {
            steps {
                echo 'Compiling code...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
}
