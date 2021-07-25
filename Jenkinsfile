pipeline {
    agent any

    options{
        skipDefaultCheckout()
    }

    stages {
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}