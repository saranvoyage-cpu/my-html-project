pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                echo 'Cloning repository...'
                git branch: 'main', url: 'git@github.com:saranvoyage-cpu/my-html-project.git'
            }
        }

        stage('Build') {
            steps {
                echo 'No build steps for static HTML project.'
            }
        }

        stage('Deploy to Client') {
            steps {
                sh 'scp -o StrictHostKeyChecking=no *.html user@192.168.1.15:/var/www/html/'
            }
        }
    }
}

