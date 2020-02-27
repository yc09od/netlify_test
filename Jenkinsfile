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
                  sh 'node --max_old_space_size=8192 ./node_modules/@angular/cli/bin/ng build'
              }
          }
      stage('deploy') {
              steps {
                  sh 'node --max_old_space_size=8192 ./node_modules/@angular/cli/bin/ng serve'
              }
          }
    }
}
