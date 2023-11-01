pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Namaskara devaru"
            }
        }
        stage('Test'){
            steps {
                sh 'bash test.sh'
            }
        }
        stage('Deploy') {
            steps {
                echo "Successfully deployed"
            }
        }
    }
}
