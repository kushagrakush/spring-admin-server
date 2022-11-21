pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        sh '/opt/apache-maven/bin/mvn clean package'
      }
    }
    stage('Deploy') {
      steps {
        sh 'opt/apache-maven/mvn deploy -DmuleDeploy'
      }
    }
  }
}
