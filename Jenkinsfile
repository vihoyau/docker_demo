pipeline {
    // agent {
    //     label 'docker' 
    // }
    agent {
        docker {
        // Set both label and image
        label 'docker'
        image 'node:7-alpine'
        args '--name docker-node' // list any args
        }
    }
    stages {
        agent {
            docker {
            // Set both label and image
            label 'docker'
            image 'node:7-alpine'
            args '--name docker-node' // list any args
            }
        }
        stage('Docker node test') {
            steps {
                // Steps run in node:7-alpine docker container on docker slave
                sh 'node --version'
                sh 'npm install'
                sh 'npm run start'
            }
        }
    }
}