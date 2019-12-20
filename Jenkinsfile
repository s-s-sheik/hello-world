pipeline {
  agent any
  stages {
    stage('Initialize') {
      steps {
        sh '''echo PATH = ${PATH}
'''
      }
    }

    stage('stage1') {
      steps {
        echo 'stage1'
      }
    }

    stage('stage2') {
      steps {
        echo 'stage2'
      }
    }

    stage('stage3') {
      when {
        expression {
          environment 'env' 'test'
        }

      }
      steps {
        echo 'stage3'
      }
    }

  }
  environment {
    env = 'test'
  }
}