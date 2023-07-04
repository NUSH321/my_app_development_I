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
    }
}