pipeline {                                                                  
  agent any                                                                 
  stages {                                                                  
    stage('--- clean ---') {                                                
      steps {
        sh "rm -rf *"
        sh "git clone https://github.com/rahul-git1/hello-world-master.git" 
        sh "/opt/maven/bin/mvn clean -f hello-world-master"                     
      }                                                                     
    }                                                                       
    stage('--- test ---') {                                                 
      steps {                                                               
        sh "/opt/maven/bin/mvn test -f hello-world-master"                      
      }                                                                     
    }                                                                       
    stage('--- package ---') {                                              
      steps {                                                               
        sh "/opt/maven/bin/mvn package -f hello-world-master"                   
      }                                                                     
    }                                                                       
  }                                                                         
}                                                                           
