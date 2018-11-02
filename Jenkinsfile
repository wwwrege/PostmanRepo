pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo 'testing this'
                step([$class: 'DockerComposeBuilder', dockerComposeFile: 'docker-compose.yml', option: [$class: 'StartService', scale: 1, service: 'translatorAcceptDocumentUpload'], useCustomDockerComposeFile: false])

            }
        }
    }
}
