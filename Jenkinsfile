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
                ./build_script.sh 'docker build -t galaxy/redis .'
            }
        }
    }
}
