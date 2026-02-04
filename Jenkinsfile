pipeline {
    agent any

    stages {
        stage('Deploy to Nginx') {
            steps {
                echo "Deploying full website to /var/www/kyqwfg.in"
                // Purana folder clear karo
                sh 'rm -rf /var/www/kyqwfg.in/*'
               // Naye code copy karo
                sh 'cp -r ${WORKSPACE}/* /var/www/kyqwfg.in/'
              // Permissions set karo
                sh 'chown -R www-data:www-data /var/www/kyqwfg.in'
                sh 'chmod -R 755 /var/www/kyqwfg.in'
            }
        }
    }
}
