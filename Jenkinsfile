pipeline {
    agent any
    stages {
        stage('Removed files') { 
            steps {
                echo 'started'
                sh '''
                ls
                pdw
                rm rf $JENKINS_HOME/workspace/*
                ls
                ''' 
            }
        }
    }
}
