pipeline {
    agent any
    stages {
        stage('Upload to AWS.') {
            steps {
                withAWS(region:'us-west-2',credentials:'1fcfe3e6-60ab-41c7-9dfc-413a256a1c03') {
                      sh 'echo "Uploading index.html to S3 bucket"'
                          s3Upload(file:'index.html', bucket:'jenkinsite')
                      }
                }

        }

    }

}