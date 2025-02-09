pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo 'building'
                sh 'docker build -t noahaviv .'
            }
        }
        stage('build2'){
            steps { 
                sh 'docker run -d -p 5000:5000 noahaviv'
                sh 'curl http://3.223.129.21:5000/'
            }
        }
    }
}
