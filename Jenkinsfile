pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t demo-ci .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run demo-ci'
            }
        }

    }
}
