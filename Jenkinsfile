pipeline {
    agent any

    stages {
        stage('compile hello') {
            steps {
                sh "cd hello; gi build"
            }
        }
        stage('compile helloserver') {
            steps {
                sh "cd helloserver; gi build"
            }
        }
        stage('compile outyet') {
            steps {
                sh "cd outyet; gi build"
            }
        }
     }
}