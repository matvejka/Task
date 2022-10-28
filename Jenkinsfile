#!/usr/bin/env groovy

pipeline {

    agent any

    stages {
        stage('Test') {
            steps {
                withKubeConfig(caCertificate: '', clusterName: 'devops-interview-aks', contextName: '', credentialsId: 'PavelConf', namespace: 'pavel', serverUrl: 'https://devops-interview-0b426a9d.hcp.westeurope.azmk8s.io:443'){
                    sh 'helm list'
                    sh 'helm lint ./charts/deploy'
                }
            }
        }
    }
}
