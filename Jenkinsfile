pipeline {
    agent any
    stages {
        stage('Authenticate') {
            steps {
                sh "echo -n ${env.DOCKER_TOKEN} | docker login -u ${env.DOCKER_USER} --password-stdin"
            }
        }
    }
}
