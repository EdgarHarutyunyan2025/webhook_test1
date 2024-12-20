pipeline {
    agent any
    triggers {
        GenericWebhookTrigger(
            genericVariables: [
                [key: 'payload', value: '$.payload']
            ],
            token: 'your-webhook-token'
        )
    }
    stages {
        stage('Process Webhook Data') {
            steps {
                script {
                    // Доступ к данным JSON
                    def payload = readJSON text: params.payload
                    echo "Received payload: ${payload}"
                }
            }
        }
    }
}

