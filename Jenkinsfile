pipeline {
    agent any
    
    stages {
        stage('build') {
            steps {
                echo 'building'
                sh 'docker build -t noahaviv .'
            }
        }
        stage('docker') {
            steps { 
                sh 'docker run -d -p 5000:5000 --name haviv noahaviv'
            }
        }
        stage('push') {
            steps {
                echo 'pushing'
            }
        }
    }
}
