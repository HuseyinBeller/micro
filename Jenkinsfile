pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                withKubeConfig(caCertificate: '', clusterName: 'EKS-1', contextName: '', credentialsId: 'k8-token', namespace: 'webapps', restrictKubeConfigAccess: false, serverUrl: 'https://0211C350FDE4AC4B0374548DD7E51A0B.gr7.eu-central-1.eks.amazonaws.com') {
                    sh "kubectl apply -f deployment-service.yml"
                }
            }
        }
    }
    
        stage('Hello') {
            steps {
                withKubeConfig(caCertificate: '', clusterName: 'EKS-1', contextName: '', credentialsId: 'k8-token', namespace: 'webapps', restrictKubeConfigAccess: false, serverUrl: 'https://0211C350FDE4AC4B0374548DD7E51A0B.gr7.eu-central-1.eks.amazonaws.com') {
                    sh "kubectl get svc -n webapps"
                }
            }
        }
    }
 
