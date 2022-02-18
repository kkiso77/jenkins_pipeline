pipeline {
  agent any
  stages {
    stage('aaa') {
      steps {
        sh 'bbb'
      }
    }

    stage('zzz') {
      parallel {
        stage('bbb') {
          steps {
            sh 'ddd'
          }
        }

        stage('ccc') {
          steps {
            sh 'ccc'
          }
        }

      }
    }

    stage('ddd') {
      steps {
        sh 'ddd'
      }
    }

  }
}