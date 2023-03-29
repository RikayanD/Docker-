pipeline {
    agent any

    stages {
        stage('Initialize'){
        def dockerHome = tool 'myDocker'
        env.PATH = "${dockerHome}/bin:${env.PATH}"
    }
        stage('Cloning git') {
            steps {
                git 'https://github.com/RikayanD/Docker-.git'
            }
        }
        stage('Building image') {
            steps {
                sh 'docker build -t galaxy/redis .'
            }
        }
    }
}
