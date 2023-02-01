pipeline {
   agent any
   stages {
      stage('clone repo') {
          steps {
              withCredentials(usernamePassword(credentialsId :jenkins-user-github ,passwordVariable: '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', usernameVariable: 'ashutosham2002' )){
              bat("""
              git config --global credential.username {GIT_USERNAME}
              git config --global credential.helper "!echo password={GIT_PASSWORD}; echo"
              git clone https://github.com/AshutoshAM2002/node-hello.git
              
              echo "pulled the code"
              """)

          }


         }

         }
      }
}