Jenkinsfile (Declarative Pipeline)
pipeline {
    agent { docker 'node:12.16.0' }
    stages {
        stage('build') {
            steps {
                sh 'npm install'
            }
        }
    }
}
