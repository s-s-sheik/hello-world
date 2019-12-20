pipeline {
  agent any
  stages {
    stage('Initialize') {
      steps {
        sh '''echo PATH = ${PATH}
echo M2_HOME = ${M2_HOME}
mvn clean'''
      }
    }

    stage('stage1') {
      steps {
        echo 'stage1'
      }
    }

  }
}