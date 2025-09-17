pipeline {
  agent any
    stages {
        stage('test'){
            steps {
                sh 'echo "running tests..."'
            }
        }

        stage('build') {
            steps {
               echo "starting build"
               sh 'docker build -t hello-world-app .'
            }
        }
        
        stage('deploy') {
            steps {
                sh 'docker run -d --name my-app -p 3000:3000 hello-world-app'
            }
        }
    }
}
