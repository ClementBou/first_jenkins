pipeline {
    agent any

    stages {
        stage('NPMBuild') {
            steps {
                sh '''
                npm install
                npm start
                '''
            }
        }
    }
}