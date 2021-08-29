pipeline {
    agent any
    stages {
        stage('node packages') { 
            steps {
                echo 'started'
                sh 'npm install' 
                echo 'installed node packages'
            }
        }
        stage('Production build'){
            steps{
                echo 'making production build'
                sh 'npm run build'
                echo 'build process is done'
            }
        }
        stage('serving'){
            steps{
                echo 'installing serve via npm'
                sh 'npm install -g serve'
                echo 'ready to serve'
                git 'serve -s build'
            }
        }
        stage('Home page'){
            steps{
                echo 'check at http://localhost:5000'
            }
        }
    }
}
