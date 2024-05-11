pipeline {
    agent { label 'Agent-1'}

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