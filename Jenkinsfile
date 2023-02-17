pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ working.cpp -o output'
                build 'PES2UG20CS314-1'
                echo 'Build Successful'
            }
        }
        stage('Test') {
            steps {
                sh './outpu'
                echo 'Testing successful'
            }
        }
    }
    post {
        always {
            echo 'Pipeline completed'
        }
        failure {
            echo 'Pipeline failed'
        }
    }
}
