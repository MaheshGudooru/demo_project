pipeline {
    agent any
    stages {
        stage("test") {
            steps {
                echo 'Hello I am active'
            }
        }
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
                echo 'jenkins execution completed'
            }
        }
    }
    post {
        success {
            echo 'success'
        }
        failure {
            echo 'failed'
        }
    }
}