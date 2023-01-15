pipeline {
    agent { label 'AzureNode'}

    stages {
        stage('Install Apache2') {
            steps {
                sh "sudo apt update"
                sh "sudo apt install apache2"
            }
        }
        stage('See Error logs') {
            steps {
                sh "sudo tail -100 /var/log/apache2/error.log"
            }
        }
    }
    
}
