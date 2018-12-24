#!/usr/bin/env groovy

pipeline {
    agent any
    stages {
        stage('Environment Variables') {
            steps {
                echo JOB_NAME
            }
        }
        stage('Build from Jenkins file') {
            steps {
                echo 'this project is built from jenkinsfile'
            }
        }
        stage('Test from jenkinsfile') {
            steps {
                echo 'test are run from the jenkinsfile'
            }
        }
        stage('Deploy from Jenkinsfile') {
            steps {
                echo 'Deployed from jenkinsfile'
            }
        }
    }  
    post {
        always {
            echo 'this blocks gets executed always'
        }
        failure {
            echo 'failure block in the post'
        }
        success {
            echo 'this block executed because the build succedded'
        }
    }
}