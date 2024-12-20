pipeline {
    agent any
    stages {
        stage('Display JSON with cat') {
            steps {
                script {
                    def filePath = "${env.WORKSPACE}/file.json"
                    
                    sh "cat ${filePath}"
                }
            }
        }
    }
}
