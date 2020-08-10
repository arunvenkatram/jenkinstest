pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo 'building the application'
            }
        }
        stage('test') {
            steps {
                echo 'testing the application'
            }
        }
    }
    post {
        always {
            echo 'something has happened in build'
        }
        success {
            echo 'build has failed'
        }
        failure {
            echo 'something has failed'
        }
    }
}
