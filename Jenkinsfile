pipeline {
    agent any
    environment {
     APP_NAME1 = "dummy app from Jenkins global env block"
    }
    
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
