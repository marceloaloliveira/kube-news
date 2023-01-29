pipeline {
    agent any

    stages {

        stage('Build Docker Image'){
            steps{
                script{
                    dockerapp = docker.build("marceloaloliveira/kube-news:${env.BUILD_ID}", '-f ./Dockerfile ./kube-news')
                }
            }
        }

    }
}