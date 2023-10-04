pipeline {
    agent any
    stages {
        stage('Load Script') {
            steps {
                script {
                    // Load the external script file
                    def externalScript = load 'myScript.groovy'

                    // Call a function defined in the external script
                    def greeting = externalScript.greet('John')
                    echo greeting // Output: Hello, John!

                    // call the variable
                   sh 'echo "Application name: ${APP_NAME}"'
                }
            }
        }
    }
}
