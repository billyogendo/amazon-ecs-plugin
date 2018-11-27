pipeline {
    agent any

    environment {
        USER_CREDENTIALS = credentials('c239234-234-234')
    }

    stages {
        stage('ssh') {
            steps {
               git branch: 'dev', credentialsId: 'c239234-234-234', url: 'git@bitbucket.org:ejbest/aaa.git'
               
                    
                }
            }
        }
    }  
    
