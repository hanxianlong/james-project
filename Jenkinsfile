pipeline {
  agent {
    docker {
      image 'maven:3.5.2-jdk-8'
    }
    
  }
  stages {
    stage('build') {
      steps {
        dir(path: 'dockerfiles/compilation/java-8/') {
          sh '''mvn package -DskipTests
'''
        }
        
      }
    }
  }
}