pipeline {
    agent { docker 'node:12.16.1' }
    stages {
        stage('init') {
            steps {
                sh 'npm install'
            }
        }
        stage('build') {
              steps {
                  sh 'npm build'
              }
          }
    }
}
