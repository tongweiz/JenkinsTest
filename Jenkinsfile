pipeline {
    agent any

    options{
        skipDefaultCheckout()
    }

    stages {
        stage('SCM') {
            userInput = input(
                message: "Ready to deploy?", parameters: [
                booleanParam(defaultValue: false, name: 'inputdev')
            ])
        }
        stage('Deploy') {
            if (userInput) {
                echo "approve ********"
            } else {
                echo "skip **********"
            }
        }
    }
}