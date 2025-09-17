pipeline: {
    agent any
    stages: {
        stage('build') {
            steps: {
               echo "starting build"
               sh 'docker build -t hello-world-app .'
            }
        }
    }
}
