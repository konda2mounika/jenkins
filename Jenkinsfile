pipeline {
    agent any    

    environment {
        ENV_URL       = "pipeline.google.com
        SSH_CRED      = credentials('SSH')
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
// Added some commits 
// Demonstrating the PollSCM  : 19 
