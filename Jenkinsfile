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
            when { 
              branch 'jenkins-setup' 
            }
            steps {
                echo 'Deploying....'
                sh 'ifconfig'
            }
        }
    }
}