pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'cp -a ./* /data/tools'
                sh 'cd ..'
                sh 'rm -rf tools'
                sh 'echo "删除成功"'
            }
        }
    }
}