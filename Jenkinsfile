pipeline {
    agent any

    environment {
        USER_CREDENTIALS = credentials('USER_PASSWORD')
    }

    stages {
        stage('ssh') {
            steps {
               git branch: 'dev', credentialsId: 'USER_PASSWORD', url: 'git@bitbucket.org:ejbest/aaa.git'
               
                    
                }
            }
        }
    }  
    
