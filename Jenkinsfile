pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            agent { 
                label 'dev-server'
            }
            steps {
                echo 'Deploying....'
                sh '''
                echo "Deployingssss..."
                ls -l
                '''
            }
        }
    }
}