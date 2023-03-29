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
                sh 'docker build -t galaxy/redis:$BUILD_NUMBER .'
            }
        }
    }
}
