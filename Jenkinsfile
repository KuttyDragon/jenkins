pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/KuttyDragon/jenkins.git'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying locally...'
                bat 'mkdir C:\\deploy'
                bat 'copy *.html C:\\deploy\\'
                bat 'copy *.css C:\\deploy\\'
            }
        }
    }
}