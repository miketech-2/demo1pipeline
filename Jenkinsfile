pipeline{
    agent any
    stages{
        stage('git-clone'){
            steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github_id', url: 'https://github.com/miketech-2/demo1pipeline.git']]])
            }
        }
        stage('practice'){
            steps{
                sh 'cal'
                sh 'cal 2025'
                sh 'date'
            }
        }
    }
}
