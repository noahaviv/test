pipeline {
    agent any
    
    stages {
        stage('build') {
            steps {
                echo 'building'
                sh 'docker build -t noahaviv .'
            }
        }
        stage('build2') {
            steps { 
                sh 'docker run -d -p 5000:5000 noahaviv'
                sh 'curl http://127.0.0.1:5000/'
            }
        }
        stage('push') {
            steps {
                echo 'pushing'
            }
        }
    }
}
