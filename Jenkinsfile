#!/usr/bin/env groovy

pipeline {

    agent any

    stages {
        stage('Test') {
            steps {
                echo 'My Name is Pavel'
                sh 'helm list'
                sh 'helm init ./deploy'
            }
        }
    }
}
