pipeline {
    agent any
      stages {
        stage ('Lint Check') {
        steps { 
           sh 'tidy -q -e *.html'
}

}
    
        stage ('Upload AWS') {
        steps {
     withAWS(credentials:'aws-static', region:'us-west-1') {
    s3Upload(file:'index.html', bucket:'jenkins-test-chip', path:'index.html')
} 
  }          
            }
         }

   }
