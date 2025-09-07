pipeline {
    agent any
/*
    environment {
        NETLIFY_SITE_ID = '0437d715-fc51-43ca-b772-5ff2b1525fe5'
        NETLIFY_AUTH_TOKEN = credentials('netlify-token')
        REACT_APP_VERSION = "1.0.$BUILD_ID"
    }
*/
    stages {

        stage ('Docker') {
            agent {
                docker {
                    image 'amazon/aws-cli:latest'
                    // args '-u root:root'
                }
            }
            steps {
                sh '''
                    aws --version --entrypoint=''
                '''
            }
        }
    }
}
