pipeline {
    agent { node 'built-in'}
    stages {
    stage('copy index.html') {
        steps {
            sh 'cp -r index.html /var/www/html/'
        }
    }
    stage('copy dev.html') {
        steps {
            sh 'cp -r dev.html /var/www/html/'
        }
    }
    stage('copy qa.html') {
        steps {
            sh 'cp -r qa.html /var/www/html/'
        }
    }
    stage('httpd-restart') {
        steps {
            sh 'service httpd restart'
        }
    }
}

