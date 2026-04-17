pipeline {
    agent any // Run on any available executor

    stages {
        stage('Build') {
            steps {
                echo 'Compiling code...'
               
            }
        }
        stage('Test') {
            steps {
                echo 'Running unit tests...'
                
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying to Production...'
               
            }
        }
    }
    
    post { 
        always { 
            echo 'I will always run, regardless of success or failure!'
        }
        success {
            echo 'Build successful!'
        }
        failure {
            echo 'Build failed. Sending notification...'
        }
    }
}
