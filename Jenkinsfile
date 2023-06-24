pipeline {
    agent any    
    environment {
        ENV_URL       = "pipeline.google.com
        SSH_CRED      = credentials('SSH')
    }
    parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
        text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')
        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')
        // choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')
        // password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
 }
    stages {
        stage('Hai') {
            steps {
                sh "echo ${ENV_URL} "  
                    
            }
        }
        stage('Hello') {
            environment {
                ENV_URL = "stage.google.com" 
            steps {
                 sh "echo hai"  
                 sh "echo Environment URL is ${ENV_URL}"
                 sh "env" 
              
            }
        }
    }
}


// Environment variables for SSH UserName & Password
// SSH_CRED_USR
// SSH_CRED_PSW

