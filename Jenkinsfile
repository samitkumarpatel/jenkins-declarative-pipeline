pipeline {
  agent any 
  stages {
     stage("iterate") {
         steps {
           sh """
            ls -al
           """
           script {
             println "Hello World!"
             def x = load "var.groovy"
             println x
           }
         }
     }
  }
}
