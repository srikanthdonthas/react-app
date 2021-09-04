pipeline {
    agent any
    stages {
        stage('Removed files') { 
            steps {
                echo 'started'
                sh '''
                ls
                pwd
                rm -rf C:\Windows\System32\config\systemprofile\AppData\Local\Jenkins\.jenkins\workspace\*
                ls
                ''' 
            }
        }
    }
}
