pipeline {
    agent any
    stages {
        stage('Load Script') {
            steps {
                script {
                   load("myScript.groovy")   
                   echo "App name: ${env.APP_NAME}"
                }
            }
        }
    }
}
