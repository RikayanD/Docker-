pipeline {
    agent any

    stages {
        stage('Cloning git') {
            steps {
                git 'https://github.com/RikayanD/Docker-.git'
            }
        }
        stage('Building image') {
            steps {
                script 'dockerImage = docker.build registry + ":$BUILD_NUMBER"'
            }
        }
    }
}
