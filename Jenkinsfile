pipeline{
  agent any 
   tools { 
      maven 'MAVEN_HOME' 
      jdk 'JAVA_HOME' 
    }
  stages {
    stage('Compile'){
      steps {
        sh 'mvn compile'
      }
    }
    stage('package'){
      steps {
        sh 'mvn package'
      }
    }

  }
}
