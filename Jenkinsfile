pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh "cp -a ${workspace} /data"
            }
        }
    }
    post {
        cleanup {
            /* clean up tmp directory */
            dir("${workspace}@tmp") {
                deleteDir()
            }
            dir("${workspace}@script") {
                deleteDir()
            }
            /* clean up our workspace */
            deleteDir()
            /* clean up script directory */
        }
    }
}