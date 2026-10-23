pipeline {
    agent any

    parameters { choice (name: 'ENVIRONMENT' ,
                         choices: ['staging','production']) }
    stages {
       stage ('checkout') { steps { checkout scm } }
       stage ('quality') { parallel {
           stage('build') { steps { bat 'echo build' } }
           stage('Lint') { steps { bat 'echo Lint' } } }
           stage('Test') { steps { bat 'echo Test' } }         
           stage('package') { steps { bat 'echo package' } }
       }
    }   
