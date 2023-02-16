pipeline {
    agent any

    stages {
        stage('checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/AshutoshAM2002/node-hello.git'
                sh echo "hello"
            }
        }
        stage('Build') {
            steps {
                sh 'docker build -t node-app .'
            }
        }
        stage('deploy') {
            steps {
                sh 'docker run -itd -p 3000:3000 node-app'
            }
        }
    }
}
