pipeline {
    agent none
    stages {
        stage('build') {
            steps {
                echo 'testing this'
                dockerNode(image: 'hcr.io/cad/forgetranslation:0.1.0-alpha', sideContainers: ['']) 
                {
                        // some block
                }
            }
        }
    }
}
