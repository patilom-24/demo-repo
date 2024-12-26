pipeline {
    agent any
    
    stages {
        // Step 1: Clone the Repository
        stage('Clone Repository') {
            steps {
                // Pull the latest code from the GitHub repository
                git branch: 'main', url: 'https://github.com/patilom-24/demo-repo.git'
            }
        }
        stage('Deploy HTML File') {
            steps {
                sh '''
                # Deploy index.html to the web server directory (e.g., /var/www/html)
                cp index.html /var/www/html/
                cp about.html /var/www/html/
                cp hello.html /var/www/html/
                '''
            }
        }
    }
}
