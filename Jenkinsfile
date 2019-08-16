pipeline {
    agent any
      stages {
        stage ('Upload AWS') {
        steps {
     withAWS(credentials:'aws-static', region:'us-west-1') {
    s3Upload(file:'index.html', bucket:'jenkins-test-chip', path:'index.html')
} 
  }          
            }
         }

   }
