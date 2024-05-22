pipeline { 
    agent {
        label "ws"
    }
    stages {
        stage('Lint Checks') {
            steps {
                sh "echo ***** Starting Style checks *******"
                sh "npm i jslint"
                sh "ls -ltr node_modules/jslint/bin"
                sh "/home/centos/node_modules/jslint/bin/jslint.js server.js || true"
                sh "echo **** Starting Style checks *******"
            }
        }
        stage('Static Code Analysis') {
            steps {
                sh "echo Starting Static code analysis"
            }
        }
    }
}