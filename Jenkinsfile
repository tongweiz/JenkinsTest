pipeline {
    agent any

    options{
        skipDefaultCheckout()
    }

    stages {
        stage('SCM') {
            steps {
                script {
                def  userInput = input(
                id: 'userInput', message: "Some important question?", parameters: [
                booleanParam(defaultValue: false, description: 'really?', name: 'myValue')
                ])
                }
            }
        }
        stage('Deploy') {
            steps {
                if (userInput) {
                    echo "approve ********"
                } else {
                    echo "skip **********"
                }
            }
        }
    }
}