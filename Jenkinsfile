pipeline {
    agent any
    stages {
        stage('Build Image') {
            steps {
                sh 'docker build -t mindgate-test:latest .'
            }
        }
        stage('Run Container') {
            steps {
                sh 'docker run --rm mindgate-test:latest'
            }
        }
    }
}
