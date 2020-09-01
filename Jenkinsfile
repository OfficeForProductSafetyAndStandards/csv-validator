pipeline {
    agent any

    stages {
        stage('PHP 7.1') {
            steps {
                sh '/usr/local/bin/composer-php7.1 install'
                sh 'php7.1 /usr/local/bin/phpunit-7'
            }
        }
        stage('PHP 7.3') {
            steps {
                sh '/usr/local/bin/composer-php7.3 update'
                sh 'php7.3 /usr/local/bin/phpunit-9'
            }
        }
        stage('PHP 7.4') {
            steps {
                sh '/usr/local/bin/composer-php7.4 update'
                sh 'php7.4 /usr/local/bin/phpunit-9'
            }
        }
    }
}

