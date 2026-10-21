pipeline {
  agent any
  stages {
    stage ('Build') { steps { echo 'Building the projects' } }
    stage ('Test') { steps { echo 'Running tests' } }
  }
  post {
    success { echo 'pipeline succeeded' }
  }
}
      
