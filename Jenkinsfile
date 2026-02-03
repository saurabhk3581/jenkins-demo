pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t jenkins-demo:latest .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run --rm jenkins-demo:latest echo "Docker OK"'
            }
        }
    }
}
