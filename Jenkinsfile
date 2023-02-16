pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES2UG20CS457-1 new.cpp'
                echo "Build Successful"
            }
        }
        stage('Test') {
            steps {
                shi './PES2UG20CS457-1'
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
