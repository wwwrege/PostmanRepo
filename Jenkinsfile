pipeline {
    agent {docker { image 'postman/newman_ubuntu1404' }}
    stages {
        stage('build') {
            steps {
                echo 'testing this'
                step([$class: 'DockerComposeBuilder', dockerComposeFile: 'docker-compose.yml', option: [$class: 'StartService', scale: 1, service: 'translatorAcceptDocumentUpload'], useCustomDockerComposeFile: false])

            }
        }
    }
}
