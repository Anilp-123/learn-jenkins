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
    }
}