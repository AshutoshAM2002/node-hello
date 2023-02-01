pipeline {
    agent any

    stages {
        stage('checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/AshutoshAM2002/node-hello.git'
            }
        }
        stage('Build') {
            steps {
                sh 'sudo su root'
                sh 'docker build .'
            }
        }
    }
}
