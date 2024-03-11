pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'teststap'
          }
        }

        stage('test par') {
          steps {
            echo 'test par'
          }
        }

      }
    }

    stage('depoly') {
      steps {
        echo 'deploy'
        sleep 10
      }
    }

  }
}