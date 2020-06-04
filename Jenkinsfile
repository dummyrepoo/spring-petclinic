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
   }
}
