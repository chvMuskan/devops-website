pipeline {
    agent any

    stages {
        stage('Deploy') {
            steps {
                sh '''
                echo "Starting deploy"
                rm -rf /var/www/html/*
                cp -r ./* /var/www/html/
                echo "Deploy done"
                '''
            }
        }
    }
}
