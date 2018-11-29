pipeline {
    agent any

    environment {
        USER_CREDENTIALS = credentials('bitbucketcred')
    }

    stages {
        stage('clone') {
            steps {
                withCredentials([usernamePassword(credentialsId: 'bitbucketcred', passwordVariable:'PASSWORD', usernameVariable:'USERNAME')]) {
               credentialsId: 'bitbucketcred', git clone https://mike9377:Mike9377@bitbucket.org/mike9377/amazon-ecs.git'
               
                }  
              }
            }
        }
    }  
    
