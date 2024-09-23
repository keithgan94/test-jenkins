pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    sh 'docker build -t python-web-app:v1 .'
                }
            }
        }
        stage('Run') {
            steps {
                script {
                    sh 'docker run -d -p 5000:5000 python-web-app:v1'
                }
            }
        }
    }
}
