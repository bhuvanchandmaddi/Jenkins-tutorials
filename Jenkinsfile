pipeline {
    agent any
    stages {
        stage('Load Script') {
            steps {
                script {
                    // Load the external script file
                    def externalScript = load 'myscript.groovy'

                    // Call the injected function
                    def greeting = externalScript.greet('John')

                    // Output the greeting to the console
                    echo greeting
                }
            }
        }
    }
}
