pipeline {
    agent any

    stages {
        stage ('Buil Docker Image') {
            steps {
                script {
                    dockerapp = docker.build("fernandostn/kube-news:${env.BUILD_ID}", '-f ./srv/Docherfile ./src')
                }
            }
        }
    }
}