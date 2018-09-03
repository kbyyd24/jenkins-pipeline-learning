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
    stage('trigger deploy production') {
      steps {
        input(message: 'It\'s OK to go live?', id: 'go-live', ok: 'Yes')
      }
    }
    stage('deploy to production') {
      steps {
        echo 'Deploying to prodocution'
      }
    }
  }
}