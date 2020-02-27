Jenkinsfile (Declarative Pipeline)
pipeline {
    agent { docker 'node' }
    stages {
        stage('build') {
            steps {
                sh 'npm install'
            }
        }
    }
}
