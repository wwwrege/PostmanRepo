pipeline {
    //agent {docker { image 'postman/newman_ubuntu1404' }}
    agent any
    stages {
        stage('build') {
            steps {
                echo 'testing this'
                //step([$class: 'DockerComposeBuilder', dockerComposeFile: 'docker-compose.yml', option: [$class: 'StartService', scale: 1, service: 'translatorAcceptDocumentUpload'], useCustomDockerComposeFile: false])
                powershell 'get-date' 
            }
        }
    }
}
