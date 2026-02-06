pipeline {
    agent any

    stages{

        stage("Cloning from Github...."){
            steps{
                script{
                    echo 'Cloning from Github...'
                    checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'jenkins-docker-github-token', url: 'https://github.com/Sakshingale/Hybrid-Anime-Recommender-System.git']])
                }
            }
        }
    }
}
