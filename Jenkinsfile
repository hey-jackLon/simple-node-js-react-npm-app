pipeline {
    agent none
    stages {

        stage('Build') { 
            agent {
                docker {
                    image 'node:6-alpine' 
                    args '-p 3000:3000' 
                }
            }
        }
        
        stages {
            stage('Build') { 
                steps {
                    sh 'npm install' 
                }
            }
        }
    }
}