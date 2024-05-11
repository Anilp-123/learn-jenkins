pipeline {
    agent { label 'Agent-1'}
     options {
        ansiColor('xterm')
    }
    stages {
        stage('Build') {
            steps {
                echo "Building..."
            }     
        }
        stage('Testing') {
            steps {
                echo "Tesing...."
                sh'''
                    pwd
                '''
            }
        }
        stage('Deploying') {
            steps {
                echo "Deploying...."
        }
    }
     post { 
        always { 
            echo 'I will always run whether job is success or not'
        }
        success{
            echo 'I will run only when job is success'
        }
        failure{
            echo 'I will run when failure'
        }
    }
}