pipeline {

    agent {

        docker {

            image 'node'

        }

    }

    stages {

        stage('Test') {

            steps {

                echo 'Testing...'
                sh 'ls'
                sh 'ls /var/jenkins_home/workspace/test'
                sh 'docker ps'
                sh 'docker images'
                sh 'ps'

            }

        }

        stage('Lint') {

            steps {

                echo 'Linting...'

            }

        }

        stage('Build') {

            steps {

                echo 'Building...'

            }

        }

        stage('Deploy') {

            steps {

                echo 'Deploying...'

            }

        }

    }

}
