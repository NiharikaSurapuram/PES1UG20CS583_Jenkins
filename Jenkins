pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o nireeksha pes1ug20cs668.cpp'
                build job : 'PES1UG20CS668-1'
                echo 'Build stage successful'
            }
        }
        stage('Test') {
            steps {
                sh './nireeksha_123'
                echo 'Test stage successful'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying "'
                echo 'Deployment successful'
            }
        }
    }
    post {
        failure {
          echo 'Pipeline failed'
                }
            
        
    }
}
