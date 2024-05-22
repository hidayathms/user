@Library('jenkins-shared-library') _
pipeline { 
    agent any
    stages {
        stage('Lint Checks') {
            steps {
                script {
                    nodejs.lintchecks()
                }
            }
        }
        stage('Static Code Analysis') {
            steps {
                sh "echo Starting Static code analysis"
            }
        }
    }
}
