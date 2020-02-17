Jenkinsfile (Declarative Pipeline)
pipeline {
    agent { docker 'node:6.3' }
    stages {
        stage('build') {
            steps {
                sh 'node --max_old_space_size=8192 ./node_modules/@angular/cli/bin/ng build --configuration=production'
            }
        }
    }
}
