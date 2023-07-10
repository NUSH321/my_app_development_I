pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo " what is Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }

        stage('Build Yolo5 app') {
   steps {
       sh '''
       aws ecr get-login-password --region eu-north-1 | docker login --username AWS --password-stdin 854171615125.dkr.ecr.eu-north-1.amazonaws.com
       cd yolo5
       docker build -t anushka-yolo5 .
       docker tag anushka-yolo5:latest 854171615125.dkr.ecr.eu-north-1.amazonaws.com/anushka-yolo5:latest
       docker push 854171615125.dkr.ecr.eu-north-1.amazonaws.com/anushka-yolo5:latest
       '''
   }
}

    }


}