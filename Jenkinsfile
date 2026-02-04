pipeline {
    agent any

    stages {
        stage('Deploy to Nginx') {
            steps {
                sh 'rm -rf /var/www/kyqwfg.in/*'
                sh 'cp -r ${WORKSPACE}/* /var/www/kyqwfg.in/'
                sh 'chown -R www-data:www-data /var/www/kyqwfg.in'
            }
        }
    }
}
