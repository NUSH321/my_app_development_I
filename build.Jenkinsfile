pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                sh '''
                    echo "BUILDING JENKINS"
                    ls -lah
                '''
            }
        }
    }
}