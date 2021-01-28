pipeline {
  agent any 
  stages {
     stage("iterate") {
         steps {
           sh """
            ls -al
           """
           script {
             def x = load "var.groovy"
             print x.helloWorld()
             
           }
         }
     }
  }
}
