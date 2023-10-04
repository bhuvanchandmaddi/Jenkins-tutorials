pipeline {
    agent any
    stages {
        stage('Load Script') {
            steps {
                script {
                    // Load the external script file
                    load 'myScript.groovy'

                    // Call the injected function
                    def greeting = greet('John')

                    // Output the greeting to the console
                    echo greeting
                }
            }
        }
    }
}
