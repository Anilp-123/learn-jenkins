pipeline{
    agent{ node 
        { 
            label 'AGENT-1' 
        } 
    } 
    stages{
        stage ('Build') {
            steps{
                ehco "Building......"
            sh '''
                ls -ltr
                pwd
                echo "Hello From Github"
            '''
            }
        }
        stage ('test') {
            steps{
                echo "Testing..."
            }
    }

        stage ('Deploying') {
            steps{
                echo "Deploying..."
            }
        }
    }
    post {
        always {
            echo "I will always run"
        }
        success {
            echo "I will Only run if the job is success"
        }
    }
}