pipeline {
    agent {
  label 'slave-machine'
}
    tools {
       maven 'maven'
       }
    
  stages  {
    
    stage(checkout){
      steps {
      git 'https://github.com/shivanani220/os-sample-java-web.git'
           }
        }
      stage(build) {
      steps {
      sh label: '', script: 'mvn clean package'
            }
        }
     } 
  }    
    
