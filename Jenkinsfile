
pipeline {
    agent any
    options {
        timeout(time: 5, unit: 'SECONDS')
    }
    stages {
        stage('Test') {
            steps {
                sh './test.sh'
            }
        }
    }
}
