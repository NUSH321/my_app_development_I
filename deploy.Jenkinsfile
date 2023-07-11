pipeline {
    agent any
    parameters { string(name: 'YOLO5_IMAGE_URL', defaultValue: '', description: '') }
    stages {
        stage('Deploy') {
            steps {
                sh '''
                echo authenticate eks cluster
                echo go to yolo5 deployment yaml file, and change the image to YOLO5_IMAGE_URL
                echo "kubectl apply -f k8s/yolo5.yaml"

            }
        }
    }
}