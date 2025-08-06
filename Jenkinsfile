
pipeline {
    agent any
    options {
        timeout(time: 1, unit: 'SECONDS')
    }
    stages {
        stage('Test') {
            steps {
                sh 'newman run test-collection.json'
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
