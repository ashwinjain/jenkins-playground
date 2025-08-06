
pipeline {
    agent any
    options {
        timeout(time: 1, unit: 'SECONDS')
    }
    stages {
        stage('Test') {
            steps {
                sh './test.sh'
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
