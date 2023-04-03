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
                sh 'def customImage = docker.build("my-image:${env.BUILD_ID}")
                    customImage.push()'
            }
        }
    }
}
