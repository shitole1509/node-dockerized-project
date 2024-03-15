pipeline {
  agent any
  stages {
    stage("checkout") {
      steps {
        checkout scm
      }
    }
    stage("Test") {
      steps {
        sh "sudo npm install"
        sh "npm test"
      }
    }
    stage("Build") { // Corrected stage name syntax
      steps {
        sh "npm run build"
      }
    }
  }
}
