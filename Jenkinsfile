pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh "aws cloudformation create-stack --stack-name webserver --template-body file://EC2.yaml --region 'ap-south-1'"
            }
        }
    }
}