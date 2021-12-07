pipeline{
  agent any 
  stages {
    stage('Compile'){
      steps {
        sh 'mvn compile'
      }
    }
    stage('package'){
      steps {
        sh 'mvn package'
        sh "mv target/*.war http://3.108.221.68:8080//addressbook.war"
      }
    }

  }
}
