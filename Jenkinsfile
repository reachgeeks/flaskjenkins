pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                git url: 'https://github.com/reachgeeks/flaskjenkins.git'
                sh 'sudo docker build -f Dockerfile -t flask-v1 .'
                sh 'sudo docker run -d -p 7000:7000 flask-v1'
            }
        }
        
        
    }
}
