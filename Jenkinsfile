pipeline {
    agent any
    stages {
        stage('Example') {
            input {
                message "Should we continue?"
                ok "Yes, we should."
                submitter "admin,anthony"
                parameters {
                    string(name: 'PERSON', defaultValue: 'Mr Anthony', description: 'Who should I say hello to?')
                }
            }
            steps {
                println "Hello, ${PERSON}, nice to meet you."
            }
        }
    }
}