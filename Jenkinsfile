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
        sh "mv target/*.war target/addressbook.war"
      }
    }

  }
}
