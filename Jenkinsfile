pipeline {
    agent any

    stages {
        stage('install') {
            steps {
                echo 'npm install'
            }
        }
        stage('Build') {
            steps {
                echo 'npm run build:ssr'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
