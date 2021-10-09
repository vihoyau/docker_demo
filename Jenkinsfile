Jenkinsfile (Declarative Pipeline)
pipeline {
    agent { docker 'node:14.17.6' }
    stages {
        stage('build') {
            steps {
                sh 'npm --version'
            }
        }
    }
}