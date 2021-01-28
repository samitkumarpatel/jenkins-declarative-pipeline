def x = load "var.groovy"

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
             println x
           }
         }
     }
  }
}
