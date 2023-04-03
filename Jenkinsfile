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
                sh 'def app = docker build -t rikayan/job1 .'
            }
        }
    }
}
