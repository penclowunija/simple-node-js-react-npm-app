pipeline {
<<<<<<< HEAD
    agent any
=======
    agent {
        docker {
            image 'node:+ docker pull node:lts-bullseye-slim'
            args '-p 3000:3000'
        }
    }
>>>>>>> parent of 26a6314 (Update Jenkinsfile)
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