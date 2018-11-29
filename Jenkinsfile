pipeline {
    agent any

    environment {
        USER_CREDENTIALS = credentials('USER_PASSWORD')
    }

    stages {
        stage('clone') {
            steps {
                withCredentials([usernamePassword(credentialsId: 'USER_PASSWORD', passwordVariable:'PASSWORD', usernameVariable:'USERNAME')]) {
               git branch: 'master', credentialsId: 'USER_PASSWORD', url: 'https://github.com/billyogendo/amazon-ecs-plugin.git'
               
                }  
              }
            }
        }
    }  
    
