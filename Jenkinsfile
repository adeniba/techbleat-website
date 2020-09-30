pipeline {
    agent any
    stages {
        stage('Copy Index File copy') {
            steps {
                echo 'I am copying index.html page'
                sh 'sudo cp index.html  /usr/share/nginx/html'
            }
        }
        stage('Copy Index jpeg file') {
            steps {
                echo 'I am copying jpeg page'
                sh 'sudo cp devops.jpg /usr/share/nginx/html'
            }
        }
        stage('Start or Status nginx') {
            steps {
                echo 'start or check status of nginx'
                sh 'sudo service nginx start'
            }
        }
                stage ('Job done') {
            steps {
                echo "task complete"
            }
        }
    }
}