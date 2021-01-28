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
                stage(k) {
                  v.each { k1,v1 ->
                    echo "for ${k} value of ${k1} is ${v1}"
                  }
                }   
             }
           }
         }
     }
  }
}
