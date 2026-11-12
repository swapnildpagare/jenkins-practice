pipeline {
    agent any

    stages {
        stage('Checkout Info') {
            steps {
                sh 'pwd'
                sh 'ls -la'
                sh 'git log -1 --oneline'
            }
        }
        stage('Build') {
            steps {
                echo 'A real Maven build will go here later'
            }
        }
    }

    post {
        success { echo 'Pipeline from Git: SUCCESS ✅' }
        failure { echo 'Pipeline from Git: FAILED ❌' }
    }
}
