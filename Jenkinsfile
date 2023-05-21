node {
  try {
    stage('Checkout') {
      checkout scm
    }

        stage('Build') {
            steps {
                        checkout scm
                        sh 'docker build -t react-backend:0.1 --no-cache .'
                        sh 'docker run -p 3000:8080 react-backend:0.1'
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

  catch (err) {
    throw err
  }
}

