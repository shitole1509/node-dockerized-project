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
        sh "sudo apt install npm"
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
