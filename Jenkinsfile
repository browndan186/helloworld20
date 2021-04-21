pipeline {
  agent any
  tools {
     maven 'M2_HOME
  }
  stages {
    stage('build'){
      steps {
        sh 'mvn clean'
        sh 'mvn install'
        sh 'mvn package'
        sleep 10
      }
    }
     stage('test'){
      steps {
        echo "test step"
        sh 'mvn test'
        sleep 10
      }
     }    
    stage('deploy'){
      steps {
        echo "deploy step"
        sleep 10
      }
    }
}
}
