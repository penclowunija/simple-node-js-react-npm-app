pipeline {
    agent any
    stages {
        stage('Back-end') {
            agent {
                  image 'maven:3-alpine'
            }
            steps {
                sh 'mvn --version'
            }
        }
        stage('Front-end') {
            agent {
                image 'node:7-alpine'
            }
            steps {
                sh 'node --version'
            }
        }
    }
}