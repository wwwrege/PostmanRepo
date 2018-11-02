pipeline {
    agent { label 'docker' }
    stages {
        stage('build') {
            agent {
                docker {
                    label 'docker'
                    image 'node:6.3'
                    args '--name docker-node'
                }
            }
            steps {
                sh 'npm --version'
            }
        }
    }
}
