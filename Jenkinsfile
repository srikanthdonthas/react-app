pipeline {
    agent any
    stages {
        stage('Removed files') { 
            steps {
                echo 'started'
                sh '''
                ls
                pwd
                cd ..
                rm -rf react-app@tmp test workspaces.txt
                ls
                ''' 
            }
        }
    }
}
