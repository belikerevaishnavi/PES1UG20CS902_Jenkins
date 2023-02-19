pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ task5.cpp'
                echo 'build stage successful'
            }
        }

        stage('Test') {
            steps {
                sh './a.out'
                echo 'test stage successful'
            }
        }

        stage('Deploy') {
            steps {
                echo 'deployed successfully'
            }
        }
    }

    post {
        failure {
                    echo 'pipeline failed'
                }
            }
        }

