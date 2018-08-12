pipeline {

    agent {

        docker {

            image 'node'

        }

    }

    stages {

        stage('Test') {

            steps {

                sh 'npm test'

            }

        }

        stage('Lint') {

            steps {

                sh 'npm run lint'

            }

        }

        stage('Build') {

            steps {

                sh 'npm run build'

            }

        }

        stage('Deploy') {

            steps {

                s3Upload(file: 'index.html', bucket: 'iabukhouski', path: 'index.html')

            }

        }

    }

}
