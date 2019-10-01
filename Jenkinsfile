pipeline {
    agent any
    stages {
        stage('Upload to AWS.') {
            steps {
                withAWS(region:'eu-west-1',credentials:'aws-static') {
                    s3Upload(file:'index.html', bucket:'jenkins-pipelite-udacity', path:'index.html')
                }
            }
        }
    }
}
