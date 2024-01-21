pipeline {
    agent any

    stages {
        stage('compile hello') {
            steps {
                sh "cd hello; go build"
            }
        }
        stage('compile helloserver') {
            steps {
                sh "cd helloserver; go build"
            }
        }
        stage('compile outyet') {
            steps {
                sh "cd outyet; go build"
            }
        }
     }
}
