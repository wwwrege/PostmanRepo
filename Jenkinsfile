pipeline {
    //agent { docker { image 'node:6.3' } }
    agent any
    stages {
        stage('build') {
            steps {
                //sh 'npm --version'
                step([$class: 'DockerComposeBuilder', dockerComposeFile: 'docker-compose.yml', option: [$class: 'StartService', scale: 1, service: 'translatorAcceptDocumentUpload'], useCustomDockerComposeFile: false])

            }
        }
    }
}
