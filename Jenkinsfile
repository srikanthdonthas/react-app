pipeline {
    agent any
    stages {
        stage(' node packages') { 
            steps {
                echo 'started'
                sh 'npm install' 
                echo 'installed node packages'
            }
            steps('Production build'){
                echo 'making production build'
                sh 'npm run build'
                echo 'build process is done'
            }
            steps('serving'){
                echo 'installing serve via npm'
                sh 'npm install -g serve'
                echo 'ready to serve'
                sh 'serve -s build'
            }
            steps('Home page'){
                echo 'check at http://localhost:5000'
            }
        }
    }
}