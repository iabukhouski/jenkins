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
                sh 'node -v'
                sh 'npm -v'
                sh 'npm test'

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
