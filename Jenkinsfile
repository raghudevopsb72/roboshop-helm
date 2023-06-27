pipeline {

  agent any

  stages {

    stage('Clone App Repo') {
      dir('APP') {
        git branch: 'main', url: 'https://github.com/raghudevopsb72/cart'
      }
    }

    stage('Helm Deploy') {
      sh 'helm upgrade -i ${component} . '
    }

  }

}