pipeline {
    agent any

    stages {

        stage ('Build Docker Image'){
            steps {
                script {
                    dockerapp = docker.build("emanuelfds/kube-news:${enb.BIOLD_ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }
    }

}