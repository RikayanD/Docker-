pipeline {
    agent any

    stages {
        stage('cloning git') {
            steps {
                git 'https://github.com/RikayanD/Docker-.git'
            }
        }
        stage('building image') {
            steps {
                script {
                dockerImage = docker.build registry + ":$BUILD_NUMBER"
                }
            }
        }
        
    }
}
