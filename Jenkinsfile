pipeline {
    agent {
        label 'nodejs'
    }

    stages {
        stage ('Install Dependencies') {
            steps {
                dir ('exchange-cli') {
                    sh "npm install"
                }
            }
        }
        stage ('Build') {
            steps {
                dir ('exchange-cli') {
                    sh "npm run build"
                }
            }
        }
    }
}