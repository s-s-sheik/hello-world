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

    stage('build') {
      steps {
        sh 'mvn -Dmaven.test.failure.ignore=true install'
      }
    }

    stage('Report') {
      steps {
        echo 'completed'
      }
    }

  }
}