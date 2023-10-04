pipeline {
    agent any
    stages {
        stage('Load Script') {
            steps {
                script {
                    // Load the external script file
                     def myScript = load 'myScript.groovy'
                      myScript.greet()              
                }
            }
        }
    }
}
