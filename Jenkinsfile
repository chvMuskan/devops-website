pipeline {
    agent any

    stages {
        stage('Deploy to Nginx') {
            steps {
                echo 'Deploying website...'
                sh '''
                rm -rf /var/www/html/*
                cp -r * /var/www/html/
                '''
            }
        }
    }
}
