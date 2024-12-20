pipeline {
    agent any
    triggers {
        GenericTrigger(
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
                    // Получаем данные из payload и выводим
                    def payload = readJSON text: params.payload
                    echo "Received payload: ${payload}"
                }
            }
        }
    }
}

