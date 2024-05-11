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
                eror
            }
        }
    }
    post {
        always {
            echo 'One way or another, I have finished'
        }
        success {
            echo 'I succeeded!'
        }
        unstable {
            echo 'I am unstable :/'
        }
        failure {
            echo 'I failed :('
        }
        changed {
            echo 'Things were different before...'
        }
    }
}