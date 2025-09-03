pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/saranvoyage-cpu/my-html-project.git', 
                    branch: 'main',
                    credentialsId: 'github-https-creds'  // we'll add this in step 2
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the project...'
            }
        }
    }
}

