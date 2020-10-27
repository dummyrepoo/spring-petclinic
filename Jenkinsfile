pipeline {
   agent {label 'MASTER'}
   stages {
      stage('source'){
         steps {
            git 'https://github.com/dummyrepoo/spring-petclinic.git'
         }
      }
      stage('package'){
         steps {
            sh 'mvn package'
         }
      }
      stage('building'){
         steps { 
            sh 'docker build image -t spc:1.0 .'
         }
      }
   }
}
