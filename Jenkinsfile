pipeline {
    agent any
    stages {
        stage('Load Script') {
            steps {
                script {
                    // Load the external script file
                    load 'myScript.groovy'

                    // Call the injected function
                    greet()

                   
                }
            }
        }
    }
}
