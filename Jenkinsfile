pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                echo 'started'
                sh 'npm install' 
                sh 'ls'
                sh '`npm run-script build'
                sh 'ls'
            }
        }
    }
}