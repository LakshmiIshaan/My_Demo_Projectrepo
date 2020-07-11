pipeline {
    agent any
    stages {
       stage("run frontend")
          steps {
            echo 'executng yarn...'
              nodejs('NodeJS10.17.0') {
                sh 'yarn install'
              }    
          }
    }   
    stage("run backend") {
       steps {
           echo 'executing gradle...'
           withGradel() {
               sh './gradel -v'
        }
     }
   }
}   
   
   
