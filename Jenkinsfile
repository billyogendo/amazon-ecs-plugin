pipeline {
    agent any

    environment {
        USER_CREDENTIALS = credentials('bitbucketcred')
    }

    stages {
        stage('clone') {
            steps {
                git branch: 'master',
                   credentialsId: '$USER_CREDENTIALS',
                   url: 'git@bitbucket.org:mike9377/amazon-ecs.git'
           }
       } 
    }
}
                
                    
