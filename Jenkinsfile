pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES1UG22CS644-1 mains.cpp'
                echo 'Build Stage Successful'
            }
        }
       stage('Test') {
    steps {
        sh './non_existent_file'
        echo 'Test Stage Successful'
    }
}

        }
        stage('Deploy') {
            steps {
                echo 'Deployment Successful'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}

