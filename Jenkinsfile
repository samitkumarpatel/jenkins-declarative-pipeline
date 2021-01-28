pipeline {
  agent any 
  stages {
     stage("iterate") {
         steps {
           sh """
            ls -al
           """
           script {
             def x = load "${env.WORKSPACE}/var.groovy"
             x.helloWorld()
             x.mapA().each { k, v ->
                echo "${k} : ${v}"
             }
             x.mapB.each { k, v ->
                echo "${k} : ${v}"
             }
           }
         }
     }
  }
}
