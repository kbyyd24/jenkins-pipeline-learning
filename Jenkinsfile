pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        git(url: 'https://github.com/kbyyd24/jenkins-pipeline-learning.git', branch: 'master')
      }
    }
    stage('deploy to stagging') {
      steps {
        echo 'Deploying to stagging'
      }
    }
    stage('deploying to production') {
      steps {
        echo 'Deploying to production'
      }
    }
  }
}