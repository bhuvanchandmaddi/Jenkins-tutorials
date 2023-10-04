pipeline {
    agent any
    stages {
        stage('Load Script') {
            steps {
                script {
                    // Load the external script file
                  //load 'myScript.groovy'
                    // Load the external script file
                    def externalScript = load 'myScript.groovy'
                    echo "Value of externalScript: ${externalScript}"
                    // Call a function defined in the external script
                    def greeting = externalScript.greet('John')
                    sh 'echo ${greeting}' // Output: Hello, John!
                    // call the variable
                   //sh 'echo "Application name: ${APP_NAME}"'
                }
            }
        }
    }
}
