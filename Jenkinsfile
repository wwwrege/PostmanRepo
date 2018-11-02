pipeline {
    agent { docker { image 'node:6.3' } }
    
    stages {
        stage('build') {
            steps {
                  container("nodeTest") {
                    script {
                       sh 'npm --version'
                    }
                
            }
        
    }
}
    }
}
