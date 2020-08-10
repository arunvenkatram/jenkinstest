pipeline {
    agent any
    environment {
        VERSION = '1.0.0'
    }
    stages {
        stage('build') {
            steps {
                echo 'building the application ${VERSION}'
            }
        }
        stage('test') {
            steps {
                echo 'testing the application ${VERSION}'
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
