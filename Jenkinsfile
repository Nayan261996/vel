pipeline {
    agent { node 'built-in'}
    stages {
    stage('copy index.htm') {
        step {
            sh 'cp -r index.html /var/www/html/'
        }
    }
    stage('copy dev.htm') {
        step {
            sh 'cp -r dev.html /var/www/html/'
        }
    }
    stage('copy qa.htm') {
        step {
            sh 'cp -r qa.html /var/www/html/'
        }
    }
    stage('httpd-restart') {
        step {
            sh 'service httpd restart'
        }
    }
}
}
