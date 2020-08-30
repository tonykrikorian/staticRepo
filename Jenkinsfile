pipeline {
    agent any
    stages {
        stage("Build") {
            steps {
                echo "Hello World!!"
                sh '''
                 echo "Multiline shell step works too"
                 ls -lah
                 '''
            }
        }
    }
}