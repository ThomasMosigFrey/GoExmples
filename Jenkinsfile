pipeline {
    agent { label "linux" }

    tools {
        go 'Go_1.21.6'
    }

    stages {

        stage('compile hello') {
            steps {
                dir('hello') {
                    sh "go build"
                    archiveArtifacts artifacts: 'hello', followSymlinks: false
                }
            }
        }

        stage('compile helloserver') {
            steps {
                dir('helloserver') {
                    sh "go build"
                    archiveArtifacts artifacts: 'helloserver', followSymlinks: false
                }
            }
        }

        stage('compile outyet') {
            steps {
                dir('outyet') {
                    sh "go build"
                    archiveArtifacts artifacts: 'outyet', followSymlinks: false
                }
            }
        }
    }
}
