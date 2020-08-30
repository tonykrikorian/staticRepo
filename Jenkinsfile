pipeline {
    agent any
    stages {
        stage("deploy"){
            steps{
                echo "Deploying ${BRANCH_NAME}"
                echo "Deploying application"
                withAWS(region: 'us-west-2',credentials:'AWS_DEV_OPS_02'){
                    echo "Login in AWS"
                    echo "Uploading to S3"
                    s3Upload(file:'index.html', bucket:'jenkins-bucket-tony', pathStyleAccessEnabled :true,payloadSigningEnabled :true)
                }
            }
        }
    }
}