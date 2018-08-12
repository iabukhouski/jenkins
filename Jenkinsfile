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

                withAWS(credentials: 'b44446e2-505b-47aa-a6a7-c560c5f812c1') {

                    s3Upload(file: 'build/', bucket: 'iabukhouski', path: '/')

                }

            }

        }

    }

}
