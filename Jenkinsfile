pipeline {
    agent any
    stages {
        stage('Build from Jenkins file ') {
            steps {
                sh 'echo "this project is built from jenkinsfile"'
            }
        }
        stage('Test from jenkinsfile') {
            steps {
                sh 'echo "test are run from the jenkinsfile"'
            }
        }
        stage('Deploy from Jenkinsfile') {
            steps {
                sh 'echo "Deployed from jenkinsfile"'
            }
        }
    }  
    post {
        always {
            sh 'echo "this blocks gets executed always"'
        }
        failure {
            sh 'echo "failure block in the post"'
        }
        success {
            sh 'echo "this block executed because the build succedded"'
        }
    }
}