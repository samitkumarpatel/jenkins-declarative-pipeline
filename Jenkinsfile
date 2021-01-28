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
             load "var.groovy"
             MapA.each { v ->
               echo "${v}"
             }
           }
         }
     }
  }
}
