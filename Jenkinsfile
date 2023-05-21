pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                   
                        sh 'docker build -t react-backend:0.1 --no-cache .'
                        sh 'docker run -d -p 3000:3000 react-backend:0.1'
            }
        }
        stage('Test') { 
            steps {
                sh '' 
            }
        }
               // post {
     //   always {
     //       cleanWs()
     //   }
}
}

