pipeline {
  agent any 
  stages {
     stage("echo") {
         steps {
             //error("Build failed because of this and that..")
             echo "Hello World"
             echo "JENKINS_HOME : ${JENKINS_HOME}"
         }
     }
  }
}
