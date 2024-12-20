pipeline {
    agent any
    stages {
        stage('Receive Webhook') {
            steps {
                script {
                    def payload = request.JSON
                    echo "Received JSON payload: ${payload}"
                }
            }
        }
    }
}
