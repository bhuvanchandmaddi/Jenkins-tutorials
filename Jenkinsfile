pipeline {
    agent any
    stages {
        stage('Load Script') {
            steps {
                script {
                    // Load the external script file
                  //load 'myScript.groovy'
                    // Load the external script file
                    def externalScript = load '/home/jenkins/workspace/Env-vars-demo/myScript.groovy'
                    def folder_name=sh (script: 'ls -rd * | head -n 1',returnStdout: true).trim()
                    def pwd=sh (script: 'pwd | head -n 1',returnStdout: true).trim()

                    echo "List of files:\n ${folder_name}"
                    echo "pwd: ${pwd}"
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
