pipeline {
    agent any

    stages {
        stage('NPMBuild') {
            steps {
                sh '''
                docker-compose build --build-arg DISCORD_TOKEN='$DISCORD_TOKEN' --build-arg APPLICATION_ID='$APPLICATION_ID' --detach --verbose
                docker-compose up -d
                '''
            }
        }
    }
}