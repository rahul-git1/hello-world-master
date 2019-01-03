pipeline {
  agent any
  stages {
    stage('--- clean ---') {
      steps {
        sh "/usr/bin/mvn clean"
      }
    }
    stage('--- test ---') {
      steps {
        sh "/usr/bin/mvn test"
      }
    }
    stage('--- package ---') {
      steps {
        sh "/usr/bin/mvn package"
      }
    }
  }
}
