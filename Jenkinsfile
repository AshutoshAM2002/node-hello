pipeline {
    agent any

 stages {
      stage('checkout') {
           steps {
             
                git branch: 'master', url: 'https://github.com/devops4solutions/CI-CD-using-Docker.git'
             
          }
        }
 }
 stage('Docker Build and Tag') {
           steps {
              
                sh 'docker build -t node-app:latest .' 
                //sh 'docker tag samplewebapp nikhilnidhi/samplewebapp:$BUILD_NUMBER'
               
          }
        }
}