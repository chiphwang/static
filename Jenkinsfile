pipeline {
    agents any
      stages {
        stage ('Build') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                   echo "Multiline shell steps work too"
                   la -lah
                   '''
               }
            }
         }
   }
