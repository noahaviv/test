jenkinsfile

pipeline {
    agent any
    stages {
        stage('Run Script') {
            steps {
                script {
                    chmod +x script.py
                    sh './script.py'
                }
            }
        }
    }
}
