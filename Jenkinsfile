pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        sh '''pwd
date
cal 2022
'''
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'build'
          }
        }

        stage('build parallel') {
          steps {
            echo 'parallel build'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
      }
    }

  }
}