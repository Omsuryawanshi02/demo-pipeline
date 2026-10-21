pipeline {
  agent any
  environment { APP_NAME = 'test' }
  stages {
    stage ('checkout') { steps { checkout scm } }
    stage ('Build') { steps { bat 'echo Building' } }
    stage ('Test') { steps { bat 'echo Running tests' } }
  }
  post {
    success { echo 'All stages passed' }
    failure { echo 'somthing failed' }
  }
}
      
