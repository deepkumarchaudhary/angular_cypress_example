pipeline {
    agent any

    tools {nodejs "node"}

    stages {
        stage('Build') {
            steps {
                sh 'node -v'
                sh 'npm build'
            }
        }
        stage('Unit Tests') {
            steps {
                sh 'npm test'
            }
        }
        stage('e2e Tests') {
            steps {
                sh 'npm run e2e'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
