pipeline {
    agent any
    parameters { 
        choice(name: 'ENVIRONMENT',choices: ['staging','production'],
               description: 'Target')
    }    
    stages {
        stage ('Tests') {
            parallel {
                stage('unit') { steps { bat 'echo Unit test' } }
                satge('Integration') {steps { bat 'echo Integration tests' } }
    }
} 
