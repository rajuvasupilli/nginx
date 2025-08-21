pipeline {
    agent any

    stages {
        stage('Install-Nginx') {
            steps {
             sh '''
                helm repo add bitnami https://charts.bitnami.com/bitnami
                helm repo update
                helm install my-nginx bitnami/nginx --namespace nginx --create-namespace
             '''
            }
        }
    }
}
