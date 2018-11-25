
pipeline {
  agent any 
  parameters {
    string(name: 'BRANCH', defaultValue: 'master')
  }
  stages {
    stage('build') {
      steps {
        sh 'date'
        echo 'building...'
        git branch: "${params.BRANCH}", url: 'https://github.com/patilmahadev/kube-exercise.git'
        echo 'build successful''
      }
    }
    stage('test') {
      steps {
        sh 'date'
        echo 'test successful'
      }
    }
    stage('deploy') {
      steps {
        sh 'date'
        echo 'deploy successful'
      }
    }
  }
}
