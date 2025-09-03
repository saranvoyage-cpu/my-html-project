pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout your GitHub repo using SSH and Jenkins credentials
                git url: 'git@github.com:saranvoyage-cpu/my-html-project.git',
                    credentialsId: 'github-ssh-key'
            }
        }
        
        stage('Build') {
            steps {
                echo 'Building the project...'
                // Add your build commands here (if any)
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the project...'
                // Add your deploy commands here (e.g., copying files)
            }
        }
    }
}

