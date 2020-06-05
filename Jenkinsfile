pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'cp -a ./* /data/tools'
            }
        }
        stage('test') {
          steps {
            sh 'cd ..'
            sh 'rm -rf tools'
          }
        }
    }
}