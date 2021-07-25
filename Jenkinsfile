pipeline {
    agent any

    options{
        skipDefaultCheckout()
    }

    stages {
        stage('SCM') {
            steps {
                userInput = input(
                id: 'userInput',message: "Ready to deploy?", parameters: [
                booleanParam(defaultValue: false, name: 'inputdev')
                ])
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