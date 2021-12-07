pipeline{
  agent any 
  stages {
    stage('Compile'){
      steps {
        sh 'mvn compile'
      }
    }
    stage('CodeReview'){
      steps {
        sh 'mvn -P metrics pmd:pmd'
      }
    }
    stage('UnitTest'){
      steps {
        sh 'mvn test'
      }
    }
    stage('MatricCheck'){
      steps {
        sh 'mvn cobertura:cobertura -Dcobertura.report.format=xml'
      }
    }
    stage('package'){
      steps {
        sh 'mvn package'
      }
    }

  }
}
