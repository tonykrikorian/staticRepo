pipeline {
    agent any
    stages {
        stage("Build") {
            steps {
                sh 'echo "Hello World!!"'
                sh '''
                 echo "Multiline shell step works too"
                 ls -lah
                 '''
            }
        }
    }
}