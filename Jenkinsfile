pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo "This is the build stage"
                sh 'echo using shell within Jenkinsfile'
                echo 'not using shell in the Jenkinsfile'
            }
        }
        stage('test') {
            steps {
                echo "This is the test stage"
                sh 'touch test.txt'
            }
        }
        stage('deploy') {
            steps {
                echo "This is the deploy stage"
                sh 'echo "Hello" > test.txt'
            }
        }
    }
}