Jenkinsfile (Declarative Pipeline)
pipeline {
    agent { docker 'node:6.3' }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}
