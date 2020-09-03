pipeline {
    agent none
    stages {
        stage('Env') {
            agent {
                docker { image 'python:3.7-buster' }
            }
            steps {
                sh '/bin/bash .ci/00200_requirements/run.sh'
            }
        }
    }
}
