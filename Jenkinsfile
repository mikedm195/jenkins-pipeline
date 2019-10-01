pipeline {
    agent any
    stages {
        stage('Upload to AWS.') {
            steps {
                withAWS(region:'eu-west-1') {
                    s3Upload(file:'index.txt', bucket:'jenkins-pipelite-udacity', path:'index.html')
                }
            }
        }
    }
}
