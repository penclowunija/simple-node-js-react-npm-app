pipeline {
    agent any
    stages {
        stage('Back-end') {
            agent {
                docker {
//                   label 'dockerserver'  // both label and image
                  image 'maven:3-alpine'
                }
            }
            steps {
                sh 'mvn --version'
            }
        }
        stage('Front-end') {
            agent {
              docker {
//                 label 'dockerserver'  // both label and image
                image 'node:7-alpine'
              }
            }
            steps {
                sh 'node --version'
            }
        }
    }
}