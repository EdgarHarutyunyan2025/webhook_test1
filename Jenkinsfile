pipeline {
    agent any
    stages {
        stage("pylint test") {
            steps{
                script {
                    def payload = readJSON text: params.payload
                    echo "Received Push Event: ${payload}"
                }    
            }
        }
    }
}

