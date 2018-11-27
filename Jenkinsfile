pipeline {
    agent any

    environment {
        USER_CREDENTIALS = credentials('USER_PASSWORD')
    }

    stages {
        stage('ssh') {
            steps {
               git branch: 'master', credentialsId: 'USER_PASSWORD', url: 'https://github.com/billyogendo/amazon-ecs-plugin.git'
               
                    
                }
            }
        }
    }  
    
