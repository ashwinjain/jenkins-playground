
pipeline {
    agent any

    stages {
        stage('Test') {
            steps {
                sh '/opt/homebrew/bin/newman run test-collection.json'
            }
        }
    }
    post {
        always {
            echo 'Job finished'
        }
        success {
            echo 'Status: success'
        }
        failure {
            echo 'You failed'
        }
    }
}
