
pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    sh 'docker build -t flask-app .'
                }
            }
        }
        stage('Run') {
            steps {
                script {
                    sh 'docker run -d -p 5000:5000 flask-app'
                }
            }
        }
    }
}
