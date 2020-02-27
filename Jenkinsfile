pipeline {
  agent { 
    docker {
      image 'node:12.16.1'
      args '-p 3000:3000'
    } }
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
