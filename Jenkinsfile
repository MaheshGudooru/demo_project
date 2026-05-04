pipeline {

    agent {
        docker {
            image 'openjdk:17'
        }
    }

    stages {

        stage('compile') {

            steps {

                sh 'javac Demo.java'

            }

        }

        stage('running') {

            steps {

                sh 'java Demo'

            }

        }

        stage('final') {

            steps {

                sh 'echo jenkins execution completed'

            }

        }

    }

    post {

        success {

            sh 'echo success'

        }

        failure {

            sh 'echo failed'

        }

    }

}