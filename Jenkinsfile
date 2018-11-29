pipeline {
    agent any

    environment {
        USER_CREDENTIALS = credentials('bitbucketcred')
    }

    stages {
        stage('clone') {
            steps {
                withCredentials([usernamePassword(credentialsId: 'bitbucketcred', passwordVariable:'PASSWORD', usernameVariable:'USERNAME')]) {
                git branch: 'master', credentialsId: 'bitbucketcred', url: 'https://mike9377@bitbucket.org/mike9377/amazon-ecs.git'
               
                }  
              }
            }
        }
    }  
    
